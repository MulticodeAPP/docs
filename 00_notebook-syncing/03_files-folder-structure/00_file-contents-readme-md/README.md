https://multicode.app/n/docs/sync/file/file-contents

# File contents (`README.md`)

The `README.md` of a file consists of three sections:
- "sync URL" to the file on Multicode
- title of the file
- (optional) markdown content

**Example**

````markdown
https://multicode.app/n/<your_notebook_id>/sync/file/<your_file_id>

# File title

```yaml
# (optional) file settings
assignments-due-date: 2022-01-01T23:59:59Z
```

... (optional) markdown content ...
````

Where:
- `your_notebook_id` = Notebook ID
- `your_file_id` = your unique ID for this file (maximum of 64 characters)

This link has two functions:
- for you to quickly navigate to the file on Multicode
- for Multicode to identify which file you are talking about

If you have assignments belonging to this file, you could add a default assignment due date to all assignments to this file. The due date can also be overwritten on a per-assignment basis.

The assignment due date has to be an ISO date string, like:
- `2022-01-01T23:59:59Z` - `Z` = UTC time
- `2022-01-01T23:59:59+01:00` - time with a `+1` hour offset