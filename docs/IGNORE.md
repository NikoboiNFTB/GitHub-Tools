# [`ignore`](/git/ignore) and [`ignore-reset`](/git/ignore-reset)

A pair of scripts to manage local Git ignore rules across all repositories in subdirectories.

#### `ignore`

Adds specified files or directories to the `git/info/exclude` file for all repositories, ignoring them locally without modifying `.gitignore`.

**Usage:**

Provide file or directory names as arguments:

```bash
./ignore file1 file2 dir1/ dir2/
```

If no arguments are given, the script will prompt for input.

#### `ignore-default`

Resets all `git/info/exclude` files to a default template, including standard comments and example patterns, effectively restoring a clean baseline for local ignores.

**Usage:**

Run the script from the parent directory containing your Git repos:

```bash
./ignore-default
```
