# Overview
this will go over basic window cli functionalities and basic cli utilities

## Changing directories

```shell
cd 

cd \
```
## changing drives
just add a `:` after the letter representind our drive
```shell
D:
```
if you know which dir to go to in a drive:
```shell
cd /D C:\Windows
```

## viewing directory contents
simply use:
```
dir
```

to view with hidden files
```shell`
dir /A
```

## mkdir
to create directories
```shell
mkdir C:\Users\User\mynewfolder
```
## copy
Copy allows us to copy one or more files to a different location, while leaving the original file untouched.

```shell
copy file1.txt file2.txt
```

if we want to copy multiple files into a new folder:
```shell
copy *.txt .\copy_target_dir
``` 
copy cannot be used to copy directories, it will copy its contents over only.

## robocopy
a command that allows you to copy files, directories, and even entire drives from one location to another.

use`/s` to copy an entire directory tree(meaning this copies the directory abd all budirectories while excluding the empty ones, which you  can use `/e` for)
```shell
robocopy source_dir dest_dir /s
```
## move
used to move one or more files from one location to another. Unlike 'copy' when using 'move' we can move directories without any extra commands.

```shell
move source_dir dest_dir
```


