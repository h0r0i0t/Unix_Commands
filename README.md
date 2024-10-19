# Unix_Commands

## ls:
### Listing Files:
### Syntax: -ls
### -R: shows all files in directories or subdirectories
### -al: gives information about files
### -a: Shows hidden files

## cat:
### Used to read contents of a file
### Syntax: cat <filename>
## rm: Removes a file/directory
### Syntax: rm <filename>
### -r: Used to remove sub-directories

## mv: 
### Used to rename and move files
### Syntax 1: mv <filename> <new_file_location>
### Syntax 2: mv <filename> <new_filename>

## sudo:
## Lets you run commands with security privilages
### Syntax: sudo <command_you_want_to_execute>

## mkdir:
### Used to make a new directory
### Syntax: mkdir <directoryname>

## rmdir:
### Used to remove a directory
### Syntax: rmdir <directoryname>

## man:
### Used to gain knowledge about any command
### Syntax: man <command>

## History:
### Used to see history

## clear:
### Used to clear console

## pr:
### Used to print the contents of a certain file
### -x <filename>: x stands for number of paragraphs
### -h "header" <filename>: used to give header to the text you are printing
### -n <filename>: numbers each line of text




















## '|'- Piping command
### Used to run 2 or more commands consecutively
### Syntax: <command>|<command>
### Example: Using the cat with less,pg or more command to scroll through the contents, as normally cat will automatically jump to the last page.,<br>
cat <filename> | less

## grep:
### Used to find a certain string in a given file
### Syntax: grep <search_string> or cat <filename> | grep <search_string>
### -v: Shows lines that didnot match the searched strings
### -c: Displays count of matching files
### -n: Shows matching line and number
### -i: Matches both uppercase and lowercase of string
### -l: Shows name of the file with the string

## sort:
### Used to sort a content of file in alphabetical order
### Syntax: sort <filename>
### -r: reverses the sorting
### -n: sorts numrically
### -f: case insensitive sorts

# Regular Expressions

## ^
### Matches to first letter of string

## $
### Matches end of string

## .
### Replaces any character

## *
### Matches upto 0 or more times the preceding character

## \
### Represents special character

## ()
### Groups regular expressions

## ?
### Matches exactly one character

## Regular Expressions:
### used to filter out by checking number of times the input is repeated
### Syntax: cat <filename> | grep -E <search_string>/{number_of_times}

## Extended Regular Expressions:
### \+: Matches one or more occourance of the previous character.
### \?: Matches zero or one occourance of the previous character.

# Brace Expansions:
## Used to generate lists
## Example: {0..5}<br>0 1 2 3 4 5

# Linux Networking Commands

## ping: 
### Used to check the connection to a server
### Syntax: ping <hostname>

## FTP: 
### Used for data transfer between computers. Can be used to navigate directories and add files to them. Downloading and Uploading files made easier.
### Syntax: ftp <hostname/ipadress>

## Telnet: 
### Used to connect to remote computers and execute. Not in use anymore since we have better and more secure ways of connecting to a remote computer.

## SSH:(Secure Shell):
### Better way to connect to remote computers, encrypts passwords.
### Syntax: SSH username@ip_adress/hostname

# Process Managing:
## top:
### Tells us all the running processess
#### PID: Process id
#### User: Username of task owner
#### PR: Priority: 20 is highest, -20 is lowest
#### NI: Nice value of task

## PS(process status):

### Used to check process staus of any process
### Syntax: PS <process_pid>
we can find process pid by using pidof <processname>

## Kill:
### terminates a given process

## Niceness:
### Used to give priority to a process
### Syntax: nice -n 'Nice Value' <processname>
### Syntax: renice 'Nice Value' -p 'PID'

## df:
### reports amount of free space in the disc
### Syntax: df

## Free:
### Shows free and used memory in Linux ststem
### Syntax: free -m/-g (for megabyte of gigabyte)
