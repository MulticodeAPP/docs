https://multicode.app/n/docs/sync/file/multiple-choice-question

# Multiple Choice Question

**Example**

````markdown
https://multicode.app/n/<your_notebook_id>/sync/assignment/<your_assignment_id>

```yaml
type: multiple_choice
points: 10 # (optional)
```

... (optional) markdown content ...
````

The answers for the question need to be specified in an `answers` folder adding the answers as separate Markdown files.

**Example**

```
\-- assignments
    \-- 02_named-assignment
        \-- README.md
        \-- answers
            \-- 01.md
            \-- 02_correct.md
            \-- 03.md
            \-- 04.md
    \-- ...
```

Answers may be ordered by using numbers in the file name.

The answer file should contain Markdown content, detailing the answer. A file containing the/a correct answer should contain the word `correct` in the file name.

The file name is also the identifier used for this multiple choice answer. It may be a maximum of 64 characters.
