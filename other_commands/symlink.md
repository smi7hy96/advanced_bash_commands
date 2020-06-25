Advanced bash

### What does ls, ll and -a do?
1. ls: list all contents of a directory
2. -a: all files and folders, including ones that are hidden and start with a
3. ll: list the detail information of files and folder of a current directory

### What is grep?
- what grep stands for | Global regular expression print
- what grep does | Search Files and Directories for Patterns of Text

- grep: Search Files and Directories for Patterns of Text
- syntax:
1. grep "pattern or code your looking for" "file.txt"
2. adding the -w before the pattern or code we are looking for, it will only return !exact! matches






- standard output - when you type the syntax below the command returns a standard output
- syntax: echo 'hello world'

### What are symbolic links in linux?
1. A symlink is a shortcut to another file.
2. A soft link (also called symbolic link) is a file system entry that points to the file name and location. Deleting the symbolic link does not remove the original
3. If however, the file to which the symbolic link points to is removed, the symbolic link stops working, it is broken
4. As similar to hard links, any changes to the data in either file is reflected in the other

### How do we create a symbolic link?
1. ln -s. If we do not include the -s, a hard link will be created
2. ln -s symlink/important.txt symlink.txt


### What are the uses for a symlink?
1. Symbolic links are used all the time to link libraries and make sure files are in consistent places without moving or copying the original. Links are often used to “store” multiple copies of the same file in different places but still reference to one file.
