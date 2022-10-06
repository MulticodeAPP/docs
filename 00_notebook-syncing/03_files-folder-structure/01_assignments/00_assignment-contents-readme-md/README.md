https://multicode.app/n/docs/sync/file/assignment-contents

# Assignment contents (`README.md`)

The `README.md` of an assignment consists of four sections:
- "sync URL" to the assignment on Multicode
- title of the assignment
- assignment settings (defined in a YAML code block)
- (optional) markdown content

**Example**

````markdown
https://multicode.app/n/<your_notebook_id>/sync/assignment/<your_assignment_id>

# Assignment title

```yaml
type: multiple_choice
```

... (optional) markdown content ...
````

Where:
- `your_notebook_id` = Notebook ID
- `your_assignment_id` = your unique ID for this assignment (maximum of 64 characters)

This link has two functions:
- for you to quickly navigate to the assignment on Multicode
- for Multicode to identify which assignment you are talking about
