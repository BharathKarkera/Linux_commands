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
