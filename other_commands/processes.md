### Advanced Bash commands

# ps (process status) command
- Used to provide information about the currently running processes, including their process identification numbers (PIDs).

# ps -aux command
- Shows all processes for all users

# grep - Global regular expression print
- It searches for a PATTERN in a given file.

`grep --help` - displays all options related this command

# What are symbolic links in linux
- It's a special kind of file that points to another file, much like a shortcut in Windows. Unlike a hard link, a symbolic link does not contain the data in the target file. It simply points to another entry somewhere in the file system.


# How to create a symbolic links


## pipes & redirection
Pipes allow you to combine commands one after the other, like a pipeline.

`|` is the 'pipe' command


`ls -1` gives a 1 column list

`less` program which lets you see output one screen at a time


`ls -1 | less` ==> output of `ls -1` = input to `less`

# Create a process and kill it
  ```
  sleep 50 &
  ```
  this will make the machine sleep for 50 seconds and it return a process id

  ```
  kill process_id
  ```
  this kills the process
