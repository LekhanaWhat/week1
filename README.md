# week1
Find the Processes running on a linux machine : ps -aux or top\
Find the users currently logged in : $who\
Find the RAM usage : /proc/meminfo or free\
Find the disk usage : df\
Find the inode usage : df -i\
Find the ulimit of a user : ulimit -Sa (showing soft limit) ; ulimit -Ha (showing hard limit)\
Find the ulimit of a process : cat /proc/PID/limits\
Find the file descriptors used by a process : lsof -a -p PID\
Find the top 5 processes by memory usage : ps aux | sort -nk +4 | tail -n 5\
Find the top 5 processes by cpu usage : ps aux | sort -nrk 3,3 | head -n 5\
Find the top 5 processes by network usage : netstat | head -9\
Find the top 5 processes by disk iops usage : 
Find the network traffic and the bandwidth usage of a machine : nload & Iftop\
Given a file as input , find the processes using that file : lsof /dev/null\
List files opened by a process : ls -l /proc/PID/fd\
List processes listening on a specific port : lsof -i : portNo.\
Find the status of a service : systemctl status httpd\
Find the zombie processes in a machine : ps -elf | grep Z\
Find the environment variables set on a machine : printenv\
Display processes started by a user ? : -htop -u {username}\
Kill a process : kill PID\
List open ports : sudo netstat -tulpn | grep LISTEN\
Find the permissions set for a file : ls -l [file name]\
List all the directories inside a directory : tree\
Display the number of files inside a directory : ls | wc -l\
Display the number of lines in a file : wc -l [filename]\
List oldest and newest file in a directory : ls -lt | tail -1 & ls -ltr | tail -1\
Display the OS and kernel information :hostnamectl\
Display the sizing (cpu cores, memory, and disk) of the machine : lshw\
