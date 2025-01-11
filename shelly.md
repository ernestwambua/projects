# Shelly

This is a simple UNIX command interpreter.
### Compilation
Your shell will be compiled this way:

~~~~~
gcc -Wall -Werror -pedantic -std=gnu89 *.c -o hsh
~~~~~

### Showcase
The shell runs in interactive mode:

~~~~~
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
~~~~~

But it can also run in non-interactive mode:

~~~~~
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
~~~~~

## Resources
* [Everything you need to know to start coding your own shell](https://alx-intranet.hbtn.io/concepts/64)
* [Approaching a Project](https://alx-intranet.hbtn.io/concepts/350)