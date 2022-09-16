https://multicode.app/n/docs/sync/file/code-question

# Code Question

**Example**

````markdown
https://multicode.app/n/<your_notebook_id>/sync/assignment/<your_assignment_id>

```yaml
type: code
points: 10 # (optional)
language: python
```

```python | initial
def sum(a, b):
    # TODO: sum `a` and `b`
    pass
```

... (optional) markdown content ...
````

`language` denotes which programming language the question uses.

The `python | initial` code block specifies that this is initial setup code that the user can use as a starting template for the assignment. Only `initial` is required here, to specify it's about initial code input, and `python` is used to allow for syntax highlighting when viewing the `README.md`.
