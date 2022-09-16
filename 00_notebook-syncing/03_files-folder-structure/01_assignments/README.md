https://multicode.app/n/docs/sync/file/assignments

# Assignments

All files in Multicode may contain assignments, even if they function as a folder.

**Example**

```
02_assignments
    \-- 01_week-1
        \-- README.md
        \-- assignments
            \-- 01
                \-- README.md
            \-- 02_named-assignment
                \-- README.md
            \-- ...
```

Assignments are placed in the `assignments` folder. Assignments contain two numbers for ordering, an underscore, and an optional assignment title. The ordering numbers are required, as they allow for an optional title. It is highly recommendable to be consistent (for your own convenience), by either giving all or no assignments in a "set" an assignment title.

The assignment title in the directory is mostly for visually identifying which contents are contained in the directory. Inside of the `README.md`, you can specify a longer/detailed assignment title which will be used when displayed.