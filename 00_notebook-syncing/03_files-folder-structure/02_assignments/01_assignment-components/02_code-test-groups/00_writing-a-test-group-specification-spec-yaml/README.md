https://multicode.app/n/docs/sync/file/writing-a-test-group-specification

# Writing a Test Group specification / `spec.yaml`

All fields at the root of this object are optional, but you must specify at least one type of test for it to be valid.
- `points`, how many points will be earned if all tests specified in this file pass
- `required`, if all of these tests are required to complete the assignment
- `include-types`, which statements must be used and within what `range` (optional, by default use a minimum of 1)
- `blocked-types`, which statements may not be used
- `variables`, which variables must be inspected and compared with the expected values
- `functions`, which functions need to be tested, and with which arguments and expected values
    - optionally a test for a function can be made private by setting `private: true`, the user will not know these tests are run beforehand, only after a private test fails only one will be made public

**Example**

```yaml
# (defaulted to `null`)
points: 50

# (defaulted to `true`)
required: false

include-types:
  # must include at least one use of the `variable` type
  - type: variable

  # must include a minimum of 1 and maximum of 4 uses of the `function` type
  - type: function
    range:
      min: 1
      max: 4

# all types that can't be used at all
blocked-types:
  - type: for_loop
  - type: while_loop

# assert the actual values of these variables match with the expected values
variables:
  - variable: a
    expected: 2
  - variable: b
    expected: 10

functions:
  # run a suite of tests for a function named `sum`
  - reference: sum
    tests:
      - arguments:
          - 1
          - 2
        expected: 3

      - private: true # (optional, by default `false`, i.e. by default a test is public)
        arguments:
          - 3
          - 5
        expected: 8
```

Available types for `include-types` and `blocked-types`:
- `import`
- `variable`
- `if_statement`
- `else_if_statement`
- `else_statement`
- `switch_statement`
- `do_statement`
- `while_loop`
- `for_loop`
- `continue_statement`
- `break_statement`
- `try_statement`
- `catch_clause`
- `finally_clause`
- `anonymous_function`
- `function_definition`
- `return_statement`
- `yield_statement`
- `class_definition`
