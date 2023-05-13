## File Operations
- `ls` - List files in the current directory.
  - Example: `ls /home/username/Documents`

- `cd` - Change the current directory.
  - Example: `cd /home/username/Documents`

- `pwd` - Print the current directory.
  - Example: `pwd`

- `touch` - Create a new, empty file.
  - Example: `touch newfile.txt`

- `cp` - Copy files or directories.
  - Example: `cp file.txt /home/username/Documents`

- `mv` - Move or rename files.
  - Example: `mv file1.txt /home/username/Documents`

- `rm` - Delete files or directories.
  - Example: `rm file.txt`

- `find` - Search for files and directories under a specified directory.
  - Example: `find /home/username -name "file.txt"`

- `chmod` - Change the permissions of a file or directory.
  - Example: `chmod 755 script.sh`

- `chown` - Change the owner and group of a file or directory.
  - Example: `chown john:users file.txt`

## Text Manipulation
- `cat` - Display the contents of a file.
  - Example: `cat newfile.txt`

- `less` - Navigate through larger files.
  - Example: `less largefile.txt`

- `grep` - Search for a specific pattern in files.
  - Example: `grep "hello" file.txt`

- `echo` - Display a line of text or value of a variable.
  - Example: `echo Hello, world!`

- `nano`, `vi`, `emacs` - Open the respective text editors.
  - Example: `nano newfile.txt`

## System Operations
- `sudo` - Perform tasks that require administrative or root permissions.
  - Example: `sudo apt update`

- `man` - Display the manual pages for other commands.
  - Example: `man ls`

- `history` - Display a list of all previously executed commands.
  - Example: `history`

- `df` - Display the amount of disk space used and available on the filesystem.
  - Example: `df -h`

- `top` - Display dynamic real-time view of a running system i.e. tasks managed by the kernel.
  - Example: `top`

- `ps` - Report a snapshot of the current processes.
  - Example: `ps aux`

- `shutdown` - Shutdown or restart the system.
  - Example: `shutdown -r now`

## Process Management
- `ps` - Display a snapshot of the current processes.
  - Example: `ps aux`

- `top` - Monitor system, processes, and resource usage in real time.
  - Example: `top`

- `htop` - Interactive process viewer (more user-friendly than `top`).
  - Example: `htop`

- `kill` - Terminate a process.
  - Example: `kill 1234` (where 1234 is the Process ID)

## File Compression and Archiving
- `tar` - Create or extract a tarball (.tar, .tar.gz, .tar.bz2 file).
  - Example: `tar cvf archive.tar directory/` (to create tarball)
  - Example: `tar xvf archive.tar` (to extract tarball)

- `gzip` - Compress or decompress .gz files.
  - Example: `gzip file.txt` (creates file.txt.gz)
  - Example: `gzip -d file.txt.gz` (decompresses to file.txt)

- `zip` / `unzip` - Create or extract .zip archives.
  - Example: `zip archive.zip file1.txt file2.txt`
  - Example: `unzip archive.zip`

## Network Operations
- `ping` - Send ICMP ECHO_REQUEST to network hosts.
  - Example: `ping google.com`

- `ifconfig` - Display or configure a network interface.
  - Example: `ifconfig`

- `netstat` - Network statistics, showing network connections, routing tables, interface statistics, etc.
  - Example: `netstat -a`

- `ssh` - Secure Shell, for secure remote login.
  - Example: `ssh username@hostname`

- `scp` - Securely copy files between hosts over SSH.
  - Example: `scp source_file username@hostname:destination_directory`

- `wget` - Non-interactive download of files from the web.
  - Example: `wget https://example.com/file.txt`

- `curl` - Transfer data from or to a server.
  - Example: `curl https://example.com`

## Shortcuts

- `~` : This is a shortcut for the home directory of the current user. For example, if the current user's name is `username`, then `~` would translate to `/home/username/`. If you're running a command as root, `~` would refer to `/root`.

    **Example:**
    ```bash
    cd ~  # This will take you to the home directory of the current user.
    ```

- `.` : This refers to the current directory. It's often used when running scripts or executables located in the current directory.

    **Example:**
    ```bash
    ./script.sh  # This will run the script.sh file located in the current directory.
    ```

- `..` : This refers to the parent directory of the current directory.

    **Example:**
    ```bash
    cd ..  # This will take you one directory up from the current directory.
    ```

- `-` : In the `cd` command, `-` refers to the previous directory.

    **Example:**
    ```bash
    cd -  # This will take you to the last directory you were in.
    ```

- `*` : This is a wildcard character that can represent any number of characters (including zero) in a filename or directory name.

    **Example:**
    ```bash
    ls *.txt  # This will list all .txt files in the current directory.
    ```

- `?` : This is a wildcard character that represents a single character in a filename or directory name.

    **Example:**
    ```bash
    ls ?.txt  # This will list all .txt files in the current directory with a single character name (like a.txt, b.txt, etc.).
    ```

- `{}` : Braces are used to define a set of characters in a filename or directory name.

    **Example:**
    ```bash
    ls {file1,file2}.txt  # This will list file1.txt and file2.txt.
    ```

- `|` : This is the pipe operator, used to use the output of one command as input to another.

    **Example:**
    ```bash
    cat file.txt | grep "hello"  # This will search for the string "hello" in file.txt.
    ```

- `>` : This is the redirection operator, used to redirect the output of a command into a file.

    **Example:**
    ```bash
    echo "hello" > file.txt  # This will write the string "hello" into file.txt.
    ```

- `>>` : This is the appending redirection operator, used to append the output of a command to a file.

    **Example:**
    ```bash
    echo "world" >> file.txt  # This will append the string "world" to file.txt.
    ```

- `&` : When used at the end of a command, it runs the command in the background.

    **Example:**
    ```bash
    command &  # This will run "command" in the background.
    ```

- `&&` : This is used to chain commands together, where the second command runs only if the first command completes successfully.

    **Example:**
    ```bash
    cd /home/username && ls  # This will change the directory to /home/username and if successful, will list the contents.
    ```

- `;` : This is used to chain commands together, where the second command runs regardless of whether the first command completes successfully.

    **Example:**
    ```bash
    cd /home/username