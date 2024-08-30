# `mkdir` Command

## Description
The `mkdir` (make directory) command is used to create new directories in Linux. You can create one or multiple directories at once, and even set permissions during the creation.

## Syntax
```bash
mkdir [options] directory_name
```

- **`directory_name`**: The name of the directory or directories you want to create.

## Options
- `-p`: Creates parent directories as needed. If a directory in the path doesn’t exist, it will be created.
- `-v`: Verbose mode, displays a message for each directory created.
- `-m`: Sets the file mode (permissions) for the new directory, using a numeric mode (e.g., 755).

## Examples
- **Basic Directory Creation**: To create a single directory:
```shell
mkdir my_directory
```
This command creates a directory named `my_directory` in the current location.

- Create Multiple Directories: To create multiple directories at once:
```shell
mkdir dir1 dir2 dir3
```
This command creates three directories named `dir1`, `dir2`, and `dir3`.
- Create Parent Directories: To create a nested directory structure:
```shell
mkdir -p /home/user/documents/projects
```
This command creates the `projects` directory along with any parent directories (documents) that don't already exist.

- **Verbose Mode**: To display messages for each directory created:
```shell
mkdir -v new_directory
```

## Example Output
```shell
mkdir: created directory 'new_directory'
```

- Set Permissions During Creation: To create a directory with specific permissions:
```shell
mkdir -m 755 secure_dir
```
## Tips
- Use the `-p` option to avoid errors when creating nested directories. It ensures that all necessary parent directories are created automatically.
- When setting permissions with the `-m` option, make sure to use the correct numeric mode to match your security needs.
- The `mkdir` command can be combined with other commands in scripts to automate directory creation as part of larger tasks.

