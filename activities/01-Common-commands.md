# 01 Common commands

In this page you will now the basic navigation,creating/deleting of files and directories,redirecting/making output in Linux CLI.

---

### Topography

In this portion we will need to understand how we will execute any commands; if the command precede with a `$` it means you need to execute the command with the `student` user, if you the command precede with a `#` it means you need to execute the command with `root` user example:

`$ echo "I am a student"` this is executed via `student` user

`# echo "I am root"` this i s executed via `root` user

---

### Basic Inspection

As a sysadmin you need to know how to know basic inspection

To look inside of a file you can use `cat <filename>`:

`$ cat /etc/resolv.conf`

To look inside of a directory you can use `ls`:

To view the contents of your current directory

`$ ls`

To view the contents of another directory use `ls <directory name>`

`$ ls /etc`

To inspect what is your current directory you can use `pwd` command

`$ pwd`

To view information of a command to use it more efficient you can use `man <command>` but because not all commands have manual entries some of them have a `--help` subcommand examples:

`$ man ls`

or

`$ ls --help`

To view who are logged in the server `who` or simply `w` will work

`$ w`

To view what user you're using, execute `whoami`

`$ whoami`

To create an output use `echo <input>` command remember single quotes `""` will echo whatever variable and symbol shortcut you will input in echo command otherwise use `''`

`$ echo "my home is $HOME"`

and

`$ echo 'my home is $HOME'`

we will work more on this in other chapters

---

### Work with Files and/or Directory

In this portion you will understand how to work with a file and/or directory.

To create a file you need to execute `touch` command,example to create a file named "my1stFile":

`$ touch my1stFile`

To delete a file you need to execute `rm` command,example to delete a file named "my1stFile".

`$ rm my1stFile`

To create a directory you need the `mkdir` command, for example if you will create a directory named "my1stDirectory":

`$ mkdir my1stDirectory`

To remove a directory you need the `rmdir` command, for example if you will remove a directory named "my1stDirectory":

`$ rmdir my1stDirectory`
