
# BASIC LINUX COMMANDS
```THERE IS LISTING OF BASIC LINUX COMMAND WILL HELP YOU IN YOUR DAILY WORKS```

# File & Navigating
 * ls – directory listing
 * ls -al – formatted listing with hidden files
 * cd dir - change directory to dir
 * cd – change to home
 * pwd – show current directory
 * mkdir dir – create a directory dir
 * rm file – delete file
 * rm -r dir – delete directory dir
 * rm -f file – force remove file
 * rm -rf dir – force remove directory dir *
 * cp file1 file2 – copy file1 to file2
 * cp -r dir1 dir2 – copy dir1 to dir2; create dir2 if it doesn't exist
 * mv file1 file2 – rename or move file1 to file2 if file2 is an existing directory, moves file1 into directory file2
 * ln -s file link – create symbolic link link to file
 * touch file – create or update file
 * cat > file – places standard input into file
 * more file – output the contents of file
 * head file – output the first 10 lines of file
 * tail file – output the last 10 lines of file
 * tail -f file – output the contents of file as it grows, starting with the last 10 lines 

# Process Management:
 * ps – display your currently active processes
 * top – display all running processes
 * kill pid – kill process id pid
 * killall proc – kill all processes named proc *
 * bg – lists stopped or background jobs; resume a stopped job in the background
 * fg – brings the most recent job to foreground
 * fg n – brings job n to the foreground

# Permissions:
 * chmod octal file – change the permissions of file to octal, which can be found separately for user, group, and world by adding:
 * 4 – read (r)
 * 2 – write (w)
 * 1 – execute (x)
 * 
 * chmod 777 – read, write, execute for all
 * chmod 755 – rwx for owner, rx for group and world

# Networking:
 * ssh user@host – connect to host as user
 * ssh -i routingapp.pem ubuntu@34.232.33.169  –connect eith pem file
 * ssh -p port user@host – connect to host on port port as user i.e(ssh amar@163.47.212.61 -p 2020)
 * ssh-copy-id user@host – add your key to host for user to enable a keyed or passwordless login
 * ping host – ping host and output results
 * whois domain – get whois information for domain
 * dig domain – get DNS information for domain
 * dig -x host – reverse lookup host
 * wget file – download file
 * wget -c file – continue a stopped download

# System Information:
 * date – show the current date and time
 * cal – show this month's calendar
 * uptime – show current uptime
 * w – display who is online
 * whoami – who you are logged in as
 * finger user – display information about user
 * uname -a – show kernel information
 * cat /proc/cpuinfo – cpu information
 * cat /proc/meminfo – memory information
 * man command – show the manual for command
 * df – show disk usage
 * du – show directory space usage
 * free – show memory and swap usage
 * whereis app – show possible locations of app
 * which app – show which app will be run by default

# Compression:
 * tar cf file.tar files – create a tar named file.tar containing files
 * tar xf file.tar – extract the files from file.tar
 * tar czf file.tar.gz files – create a tar with Gzip compression
 * tar xzf file.tar.gz – extract a tar using Gzip
 * tar cjf file.tar.bz2 – create a tar with Bzip2 compression
 * tar xjf file.tar.bz2 – extract a tar using Bzip2
 * gzip file – compresses file and renames it to file.gz
 * gzip -d file.gz – decompresses file.gz back to file

# Installation:
 * dpkg -i pkg.deb – install a package (Debian)
 * rpm -Uvh pkg.rpm – install a package (RPM)

# Shortcuts:
 * Ctrl+C – halts the current command
 * Ctrl+Z – stops the current command, resume with
 * fg in the foreground or bg in the background
 * Ctrl+D – log out of current session, similar to exit
 * Ctrl+W – erases one word in the current line

# Screen:
```With the Linux screen command, you can push running terminal applications to the background and pull them forward when you want to see them. It also supports split-screen displays and works over SSH connections, even after you disconnect and reconnect!```

Installion:
sudo apt install screen

Description	Command
* screen -S <session_name> – Start a new session with session name
* screen -ls – List running sessions / screens
* screen -x – Attach to a running session	
* screen -r <session_name> – Attach to a running session with name	
* screen -d <session_name> – Detach a running session	
* screen -X -S [session # you want to kill] kill  – Kill a running session	
* screen -r -d [session name] – Accessing a screen that is already attached

Shortcut keys Options For Screen:
* Ctrl-a + d – It detach a screen session without stopping it.	 


# Others Important:
sudo lsof -t -i tcp:8000 | xargs kill -9  –kill running  port/ server *8000 is a port


