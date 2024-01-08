# Linux_commands

TO CHANGE SHELL :

chsh -s /usr/bin/bash


CREATING A LINK :

ln -s source_file.txt link_name


ALIAS AND DATE COMMAND:

alias dt='date +"%d-%b-%Y %A %H:%M:%S"'


INPUT OUTPUT AND ERROR REDIRECTION:

ls -lt bharath 1>ping4.txt 2>&1


SORT COMMAND :

df | sort -n -k 3 -r
cat ping.txt| sort -k1,1 -k2,2 -n   


UNIQ COMMAND:

cat ping.txt| sort | uniq -c


CUT COMMAND:

sed -n '15,30p' /etc/passwd  | cut -d ':' -f 5 | cut -c 1-4


SHELL VARIABLES :

$? --> Exit status of the last command
$$ --> PID of the current shell. For shell scripts, this is the process ID under which they are executing.
$! --> PID of the last background command/process.
$# --> Number of arguments passed to the shell script
$_ --> Last argument supplied in the last command.
$0 --> Current file name 
$1 --> First argument passed to the script
$2 --> 2nd argument passed to the script.
$* --> This parameter gives all arguments passed to the shell script separated by the space
$@ --> This parameter gives all arguments passed to the shell script separated by the space
"$*" special parameter takes the entire list as one argument with spaces between i.e.if script receives 3 arguements then "$*" --> "$1 $2 $3"
"$@" special parameter takes the entire list and separates it into separate individual arguments i.e. if script receives 3 arguements then "$@" --> "$1" "$2" "$3".

