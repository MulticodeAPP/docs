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

# (optional) assignment settings
due-date: 2022-01-01T23:59:59Z
```

... (optional) markdown content ...
````

Where:
- `your_notebook_id` = Notebook ID
- `your_assignment_id` = your unique ID for this assignment (maximum of 64 characters)

This link has two functions:
- for you to quickly navigate to the assignment on Multicode
- for Multicode to identify which assignment you are talking about

Every assignment may have a due date. It may be set on the file containing the assignments, to set a default due date for all assignments at once. Or you can overwrite/set due dates on a per-assignment basis.

The assignment due date has to be an ISO date string, like:
- `2022-01-01T23:59:59Z` - `Z` = UTC time
- `2022-01-01T23:59:59+01:00` - time with a `+1` hour offset