use piping and redirection to create powerful workflows that will automate your work, saving you time and effort.

Option	Function
-v	Shows all the lines that do not match the searched string
-c	Displays only the count of matching lines
-n	Shows the matching line and its number
-i	Match both (upper and lower) case
-l	Shows just the name of the file with the string

Option  Function

-r      Reverses  sorting

-n      Sorts numerically

-f      Case insensitive sorting

the above commands allow you to search and sort e.g

cat sample | grep -v a | sort - r

vagrant@ubuntu-xenial:~$ ls > myoutput # creates new file if none exists, creates a record of filenames within a folder

vagrant@ubuntu-xenial:~$ ls # check updated contents
ebooks_vm_pj  myoutput  node_modules  public_html

vagrant@ubuntu-xenial:~$ cat myoutput # check contents of new file
ebooks_vm_pj
myoutput
node_modules
public_html
vagrant@ubuntu-xenial:~$ ls > new_output
vagrant@ubuntu-xenial:~$ cat new_output
ebooks_vm_pj
myoutput
new_output
node_modules
public_html


vagrant@ubuntu-xenial:~$ wc -l new_output > myoutput
vagrant@ubuntu-xenial:~$ cat myoutput
5 new_output
vagrant@ubuntu-xenial:~$ ls
ebooks_vm_pj  myoutput  new_output  node_modules  public_html
vagrant@ubuntu-xenial:~$ cat new_output
ebooks_vm_pj
myoutput
new_output
node_modules
public_html


vagrant@ubuntu-xenial:~$ ls >> myoutput # appends data to a file, does not clear contents first
vagrant@ubuntu-xenial:~$ cat myoutput
5 new_output
ebooks_vm_pj
myoutput
new_output
node_modules
public_html

vagrant@ubuntu-xenial:~$ wc -l myoutput
6 myoutput #
vagrant@ubuntu-xenial:~$ wc -l < myoutput
6 # redirects data to a file

vagrant@ubuntu-xenial:~$ nano new_output # check the contents of the file

vagrant@ubuntu-xenial:~$ wc -l < new_output > myoutput
vagrant@ubuntu-xenial:~$ cat myoutput
5 # redirect and check input into a file

vagrant@ubuntu-xenial:~$ echo 'hello world'
hello world
vagrant@ubuntu-xenial:~$ echo 'hello world' > text.file
vagrant@ubuntu-xenial:~$ cat text.file
hello world
vagrant@ubuntu-xenial:~$ echo 'hello world' > text.txt
vagrant@ubuntu-xenial:~$ cat text.txt
hello world # writing into a text file from command line

grep –r “function” * recursive search

fgrep –f file_full_of_patterns.txt file_to_search.txt - specific string

grep –n “main” setup..py

ifconfig | grep –c inet6 count instances

dpkg -l | grep -i python search for instances of a file
