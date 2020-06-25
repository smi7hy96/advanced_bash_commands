## Commands
- ls: list all contents of a directory
-	-a: all files and folders, including ones that are hidden and start with a.
-	ll: list the detail information of files and folder of a current directory

## Grep

Grep searches the given files for lines containing a match to a given pattern list - search words or strings in text files.
	◦	syntax: grep 'word-to-search' filename


## Reidrect streams

### 3 streams in Linux

- standard input keyboard
- standard output what the application has
- standard error - error application has

i.e.: echo 'hello world' through command line into directory - when the command line returns it it is a standard output

Use stre-redirection to redirect a stream and create a file from scratch:
i.e. echo 'hello world' > testfile.txt (file doesn't exist but it will be created)

There is no output in command line because it had been redirected.

You can use cat, i.e. cat testfile.txt to see the output.

To append content:
i.e. echo 'hello world' >> testfile.txt

## Links

These are shortcuts.

### Soft Links (symbolic links)
- syntax : ln -s
You can make links to files and directories, and you can create links (shortcuts) on different partitions and with a different inode number than the original.

If the real copy is deleted, the link will not work.

### Hard Links
- syntax: ln /scripts/firefox /scripts/on-fire
       ( Source )    ( Destination )
Hard links are for files only; you cannot link to a file on a different partition with a different inode number.

If the real copy is deleted, the link will work, because it accesses the underlying data which the real copy was accessing.

## Permissions

- syntax: ls -l

This will show the current permissions for files and folders.
The output will resemble:
