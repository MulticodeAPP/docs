https://multicode.app/n/docs/sync/file/code-solutions

# Code Solutions

Code assignments may contain zero or more solutions, you can add them by creating a `solutions` folder and adding solutions as separate Markdown files.

**Example**

```
\-- assignments
    \-- 02_named-assignment
        \-- README.md
        \-- solutions
            \-- 01.md
            \-- 02_named-solution.md
    \-- ...
```

Solutions contain two numbers for ordering, an underscore, and an optional solution title. The ordering numbers are required, as they allow for an optional title.

The Solution file may start with an optional solution title. The Solution file must contain a code block with code that solves the assignment, followed by optional Markdown content explaining the solution.

**Example**

````markdown
# Your Solution Title

```python
def sum(a, b):
    return a + b
```

By using the `+` operator, we can add/sum multiple values.
````
