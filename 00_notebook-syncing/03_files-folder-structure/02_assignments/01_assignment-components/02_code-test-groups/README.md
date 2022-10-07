https://multicode.app/n/docs/sync/file/code-test-groups

# Code Test Groups

Code assignments may contain zero or more test groups, you can add them by creating a `test-groups` folder.

**Example**

```
\-- assignments
    \-- 02_named-assignment
        \-- README.md
        \-- test-groups
            \-- 01
                \-- README.md
                \-- spec.yaml
            \-- 02_named-test-group
                \-- README.md
                \-- spec.yaml
    \-- ...
```

Test groups contain two numbers for ordering, an underscore, and an optional test group name. The ordering numbers are required, as they allow for an optional name.

A test group will contain:
- (optional) `README.md`, containing a title for the test group and Markdown content describing the test group
- `spec.yaml`, a "spec" (specification) describing all tests that need to be executed within this test group
- (optional) `hints` folder, containing hints as specified previously
