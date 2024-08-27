# `cp` Command

## Description
The `cp` command is used to copy files and directories in Linux. It creates a duplicate of the specified file or directory at a different location.

## Syntax
```bash
cp [options] source destination
```
- `source`: The file or directory you want to copy.
- `destination`: The location where you want to copy the file or directory.

## Options

- `-r` or `-R`: Recursively copy directories and their contents.
- `-v`: Verbose mode, showing the files being copied.
- `-i`: Interactive mode, prompts before overwriting files.
- `-u`: Copy only when the source file is newer than the destination file or when the destination file is missing.
- `-f`: Force the copy by removing the destination file if it exists.

## Examples
- **Basic File Copy**: To copy a file from one location to another:
```shell
cp file.txt /home/user/documents/
```
This command copies `file.txt` to the `/home/user/documents/` directory.
- **Copy a Directory**: To copy an entire directory and its contents:
```shell
cp -r /home/user/documents /home/user/backup/
```
This command copies the `documents` directory and all its contents to the `backup` directory.

- **Verbose Mode**: To see the files being copied:
```shell
cp -v file.txt /home/user/documents/
```
## Example output
```shell
'file.txt' -> '/home/user/documents/file.txt'
```

- **Interactive Mode**: To prompt before overwriting files:
```shell
cp -i file.txt /home/user/documents/
```
Confirmation will be asked before overwriting any existing files.

- **Copy Only Newer Files**: To copy only if the source file is newer than the destination file:
```shell
cp -u file.txt /home/user/documents/
```