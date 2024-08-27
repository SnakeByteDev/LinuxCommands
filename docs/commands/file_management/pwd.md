# `pwd` Command

## Description
The `pwd` (print working directory) command is used to display the current working directory in the terminal. It shows the full path from the root directory to your current directory.

## Syntax
```bash
pwd [options]
```

## Options
- `-L`: Prints the logical current working directory, resolving any symbolic links.
- `-P`: Prints the physical current working directory, with all symbolic links resolved.

## Examples
- **Basic Usage**: To simply display our current directory
```bash
pwd
```
## Example Output
```bash
/home/user/projects
```
- `-L`: If current directory is a symbolic link, and want to display the logical path:

```bash
pwd -L
```
- `-P`: To display the physical path, resolving any symbolic links:
```bash
pwl -P
```