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

```shell
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

## del
use it to delete stuff, be careful, it does not prompt for confirmation, but using `/P` should help you with that and you should consider using it always

```shell
del /P *.txt
```

## rmdir
remove directories. if a dir is not empty it wont allow it, but you can use the `/S` flag to override that behavior
```shell
rmdir /S Demo
```
## more

used to display the contents of a file one page at a time. It works much the same as the more command from Linux. A good use of 'more' is where a command has a large output and you wish to page through it.

```shell
dir "c: \Windows" | more
```
## find
'find' searches inside files for a specified string of text. After searching the files, 'find' displays any lines of text that contain the search string. 

```shell
find c:\Users\User\* "hello" 2> nul
```
## where 
roughly equivalent to the linux one, use it to locate files on a computa

```shell
where "file*.txt"
```
default behavior can be changed by using the `/R` switch and specifying a directory; this will cause 'where' to search this directory and all sub directories for the file. 

```shell
where /R . "file*.txt"
```

