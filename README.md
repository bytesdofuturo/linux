<h1 align="center">BASIC LINUX COMMANDS</h1>

### FILES & NAVIGATING

Is - directory listing list all files/folders on current dir)
Is -| - formatted listing
Is -la - formatted listing including hidden files cd dir - change directory to dir (dir will be directory name) cd- - change to parent directory cd./dir - change to dir in parent directory cd - change to home directory pwd - show current directory mkdir dir - create a directory dir rm file - delete file rm-f dir - force remove file rm -r dir - delete directory dir rm-rf dir - remove directory dir
rm-rf / - launch some neuclear bombs targeting your system cp filel file2 - copy filel to file2
mv filel file2 - rename filel to file2
mv filel dir/file2 - move filel to dir as file2 touch file - create or update file cat file - output contents of file cat › file - write standard input into file cat » file - append standard input into file tail -f file - output contents of file as it grows

### SYSTEM INFO

date - show current date/time uptime - show uptime
whoami - who you're logged in as
w - display who is online cat /proc/cpuinfo - display cpu info cat /proc/meminfo - memory info free - show memory and swap usage du - show directory space usage du-sh - displays readable sizes in GB
df - show disk usage uname-d - show karnel config

### COMPRESSING

tar of file.tar files - tar files into file.tar tar xf file.tar - untar into current directory tar tf file.tar - show contents of archive
options:
c - create archive
t - table of contents
x - extract
z - use zip/gzip
f - specify filename
j- bzip2 compression
w - ask for comfirmation
k - do not overwrite
T - files from file
v - verbose

### SSH (Secure Shell)

ssh user@host # Connect to host as user
ssh -p port user@host # Connect using a specific port ssh-keygen -t rsa # Generate rsa key pair
ssh-copy-id user@host # Copy your key to the remote server for password-less login

### NETWORKING

ping host - ping host
whois domain - get whois for domain dig domain - get DNS for domain dig -x host - reserve lookup host wget file - download file
wget -c file - continue stopped download wget -rurl - recurively download files from url curl url - outputs the webpage from url curl-o meh.html url - writes the page to meh.html ssh user@host - connect to host as user ssh-p port user @host - connect using port ssh-D user@host - connect & use bind port

### PERMISSIONS

chmod octal file - change permissions of file
4 - read (r)
2 - write (w)
1 - execute (x)
order: owner/group/world chmod 777 - rwx for everyone
chmod 755 - w for owner, x for group world

### SEARCHING
grep pattern files # Search for pattern in files grep
-r pattern dir # Recursively search for pattern in dir find /dir -name name* # Find files starting with name in dir locate file_name # Find files by name (uses a database)

### PROCESSES
ps - display currently active processes ps aux - detailed outputs
kill pid - kill process with process id (pid) killall proc - kill all processes named proc

### SOME OTHERS
grep pattern files - search in files for pattern grep -r pattern dir - search for pattern recursively in dir locate file - find all instances of file whereis app - show possible localtions of app man command - show manual page for command
