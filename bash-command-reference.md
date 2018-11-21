### Bash Command Reference

### ls
Lists the folder and file names in the current working directory.

`ls -a` lists all files including hidden files

`ls -A` lists all files, including hidden files, except a top directory

`ls -F` add an indicator (one of */=>@|) to entries

`ls -S` sort by file size

`ls -al` provides a list of all the files in the same directory

`ls -l` Use a long listing format

`ls -nl` Use a long listing format with user ID

`ls -c` list contents by columns

### PWD
Command prints the name of working directory.

`pwd`

### CD
Changes the current working directory.

`cd /` goes to the root directory

`cd ..` goes to a parent directory

`cd` goes to the user's home directory when executed without the parameter

`cd ~root` goes to the user's home directory when the user name is given after the ‘~’

### HOME
Displays the path of the home directory.

`echo $HOME`

### NANO
Command line text editor and only accepts keyboard input.

`nano myscript.sh`

### FIND
Searches for files and directories.

`find directory -name filename`: searches the file by name

`find directory -cnewer file`: The file was last changed more recently than the file was modified

`find directory -amin n`: The file was last accessed n minutes ago

`find directory -cmin n` : The file was last changed n minutes ago

`find directory -atime n`: The file was last accessed more n days ago

`find directory -mtime n`: File’s data was last modified n days ago

`find directory -ctime n`: The file was last changed more than n days ago

`find directory -print`: Displays the path name of the files found by using the rest of the criteria

`find directory -exec`: Executes commands on the resulting search results

### MKDIR
Creates directories with this command.

`mkdir folder`: This command would create the sub folders

### MV
Moves a file or directory as another file and directory.
The commands below move file(s) from `source` directory to current.

`mv -i source`: Prompt before overwriting an existing file
`mv -f source`: Always overwrite existing files without prompting
`mv -n source`: Never overwrite any existing file
`mv -v source`: Print source and destination files

### RM
Removes objects.

`rm -f file`: Does not ask questions during deletion, does not provide information for a non-existent file

`rm -i file`: Prompt before deleting files

`rm -r directory`: Deletes the contents of directories and subdirectories consecutively

`rm -v file`: Gives more detailed information about the remove process

### RMDIR
Removes directory, this command only works if the folders are empty.

`rmdir -p directoryname`

### TOUCH
Creates or opens a file and saves it without any change to the file contents.

`touch -a file`: Updates file access time

`touch -c file`: If the file does not exist, it creates the file

`touch -m file`: Changes the file modification time

`touch -t file`: Changes the file access or replacement time as specified

### CAT
Shows the contents of the files.

`cat -n file`: Prints the contents of the file on the screen by giving a number to all lines

### WC
Prints newline, word, and byte counts for each FILE, and a total if more than one FILE is specified

`wc -l file`: Returns the number of rows

`wc -m file`: Returns the number of characters

`wc -w file`: Counts the number of words

### HEAD
Displays the first lines of lines of the file.

`head file`: Shows the first couple lines

### TAIL
Displays the last couple of lines of the file.

`tail file': Shows you the last couple lines

### MORE
The contents of the file are used to display the page page.

`more file`

### LESS
Allows backward movement in the file as well as forward movement.

`less file`

### NL
Adds a line number per line.

`nl file`

### GREP
Searches files for lines that match a pattern and returns the results.

`grep "keyword" file.tx` searches for the given string in a single file

`grep -i "keyword" file.tx` enables the command to be case insensitive

`grep -R "keyword" file.tx` searches all files in a directory and outputs filenames and lines containing matched results

### AWK
Extracts just a list of specific things.

`awk {keyword} file.tx`

### OPEN
Opens current folder in finder.

`open .`

### CHGRP
Changes the group of the file and directory.

`chgrp groupname file.txt`

### MAN
It is the interface used to view the system’s reference manuals.man ls also displays all the options available for running the command.

`man` - Print a help message and exit

`man -V --version` Display version information and exit

`man -C` Use the configuration file rather than the default of ~/.manpath.

`man -d` Print debugging information.

### ENV
Returns a list of the environment variables for the current user.

`env`