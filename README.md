# week1
1) Find the Processes running on a linux machine : ps -aux or top \
2) Find the users currently logged in : $who \
3) Find the RAM usage : /proc/meminfo or free \
4) Find the disk usage : df \
5) Find the inode usage : df -i \ 
6) Find the ulimit of a user : ulimit -Sa (showing soft limit) ; ulimit -Ha (showing hard limit)  \
7) Find the ulimit of a process : cat /proc/PID/limits \
8) Find the file descriptors used by a process : lsof -a -p PID\
9) Find the top 5 processes by memory usage : ps aux | sort -nk +4 | tail -n 5\
10) Find the top 5 processes by cpu usage : ps aux | sort -nrk 3,3 | head -n 5\
11) Find the top 5 processes by network usage : netstat | head -9\
12) Find the top 5 processes by disk iops usage : dstat -d\
13) Find the network traffic and the bandwidth usage of a machine : nload & Iftop\
14) Given a file as input , find the processes using that file : lsof /dev/null\
15) List files opened by a process : ls -l /proc/PID/fd\
16) List processes listening on a specific port : lsof -i : portNo.\
17) Find the status of a service : systemctl status httpd\
18) Find the zombie processes in a machine : ps -elf | grep Z\
19) Find the environment variables set on a machine : printenv\
20) Display processes started by a user ? : -htop -u {username}\
21) Kill a process : kill PID\
22) List open ports : sudo netstat -tulpn | grep LISTEN\
23) Find the permissions set for a file : ls -l [file name]\
24) List all the directories inside a directory : tree\
25) Display the number of files inside a directory : ls | wc -l\
26) Display the number of lines in a file : wc -l [filename]\
27) List oldest and newest file in a directory : ls -lt | tail -1 & ls -ltr | tail -1\
28) Display the OS and kernel information :hostnamectl\
29) Display the sizing (cpu cores, memory, and disk) of the machine : lshw\n
30) Find the uptime of the machine : -uptime
