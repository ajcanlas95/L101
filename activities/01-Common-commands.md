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

To change the directory use `cd` or change directory command

`$ cd /etc`

---

### Work with Files and/or Directory

In this portion you will understand how to work with a file and/or directory.

To create a file you need to execute `touch` command,example to create a file named "my1stFile":

`$ touch my1stFile`

If you want to create multiple files in one execution, you can execute `touch` command with multiple sub-parameters, for example i want to create files named "File1","File2",and "File3".  

`$ touch File1 File2 File3`

To delete a file you need to execute `rm` command,example to delete a file named "my1stFile".

`$ rm my1stFile`

Also the multiple sub-parameters in `touch` in creating also applies to `rm`, example if i want to remove files named "File1","File2",and "File3".

`$ rm File1 File2 File3`

To create a directory you need the `mkdir` command, for example if you will create a directory named "my1stDirectory":

`$ mkdir my1stDirectory`

If you want to create multiple directories in one execution, you can execute `mkdir` command with multiple sub-parameters, for example i want to create directories named "Dir1","Dir2",and "Dir3".  

`$ mkdir Dir1 Dir2 Dir3`

To remove a directory you need the `rmdir` command, for example if you will remove a directory named "my1stDirectory":

`$ rmdir my1stDirectory`

Also the multiple sub-parameters in `mkdir` in creating also applies to `rmdir`, example if i want to remove files named "Dir1","Dir2",and "Dir3".

`$ rmdir Dir1 Dir2 Dir3`

---

### Redirecting results

In this portion you will understand how redirection in Linux workshop,
in Linux there are 2 types of output:

- `stdout`
- `stderr`

`stdout` is the output if the command is successful or/and simply normal output

`stderr` is the output if the command encountered errors or/and simply an alert output

Redirecting outputs is useful such as logging and referencing etc.
For you to redirect the output from a command to a file you need to use `>` in between the command and file.

Example:

`$ echo "Linux is great" > file` this would remove all the contents of the file and replace it its content with the output.

For you to redirect output and append it you need to use `>>` in between the command and filename.

Example:

`$ echo "Linux is awesome" >> file`

by default you will redirect `stdout` for you to specify it you need to use `1>`, if you want the `sterr` just use `2>`, but if you want to capture both just use `&>`.

Example:

`$ cat /etc/resolv.conf 1> outfile` redirecting `stdout`

`$ mkdir -pv /root/awesome 2> errorfile` redirecting `stderr`

`$ mkdir -pv awsome /root/awesome &> file` redirecting both `stdout` and `stderr`

---

### Test your knowledge

As you have learn the Common commands in Linux we need to gauge if you're ready for the next part click [here](https://github.com/ajohnsc/L101/blob/master/exercise/01-Common-commands.md) for your first exercise
