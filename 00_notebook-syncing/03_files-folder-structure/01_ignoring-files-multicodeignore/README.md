https://multicode.app/n/docs/sync/file/ignoring-files

# Ignoring files (`.multicodeignore`)

The `.multicodeignore` file can be used to ignore files within the repository that shouldn't be included in the Multicode notebook. This file needs to be placed at the root of your repository, just like a `.gitignore`.

**Example**

```bash
contribution.md
images/
docs/file.md

# comments
**/files/
**/notes.md

**/dir/file.md
```

Files relative to the root of the repository can be specified by using the exact file path. Like `contribution.md`, `images/` or `docs/file.md`.

By prefixing with `**/`, you can ignore all matching files within the whole repository. Like all `notes.md` files within the whole repository, or all files placed in `files/`, and `week-1/files/`. Or also match parents of files, like `dir/file.md`, and `week-1/dir/file.md`.

Optionally use comments, prefixed with a `#`, and whitespaces as desired.

Files or directories starting with a `_` or `.` will automatically be ignored. For example: `.gitignore` and `_private/`.