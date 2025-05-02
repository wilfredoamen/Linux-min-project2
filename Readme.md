# Linux Command Project

##  Creating a Folder with sudo

- Command: `mkdir /root/example`
  - Result: `mkdir: cannot create directory ‘/root/example’: Permission denied`
- Explanation: Regular users lack permissions to create directories in `/root`.
- Command: `sudo mkdir /root/example`
  - Result: Successfully creates the folder (may prompt for password).
- Verification: `sudo ls /root`
  - Result: Lists contents, including the new `example` folder.

  ![Creating-a-Folder-with-sudo](screenshot_1-8.png)

## Understanding Linux Directory Structure

- Command: `pwd`
  - Result: `/Users/dareyio/Desktop`
- Explanation: Shows the current working directory.
- Command: `sudo cd /`
  - Followed by: `pwd`
    - Result: `/`
- Command: `sudo ls -l`
  - Result: Lists files and directories in the root filesystem (e.g., `Applications`, `Library`, etc.).

  ![Understanding-Linux-Directory-Structure](screenshot_9-17.png)

## Navigation and Side Hustle Task 1

- Command: `sudo cd /usr`
  - Followed by: `pwd`
    - Result: `/usr`
- Command: `sudo ls -l`
  - Result: Lists contents like `bin`, `lib`, `sbin`, etc.
- Task 1:
  - Command: `sudo mkdir /usr/photos`
  - Command: `sudo cd /usr/photos`
  - Command: `sudo mkdir dir1 dir2 dir3`
  - Command: `sudo ls`
    - Result: Shows `dir1`, `dir2`, `dir3`
  - Command: `sudo cd dir1`
  - Command: `pwd`
    - Result: `/usr/photos/dir1`

![Screenshot 18-25](screenshot_18-25.png)

## File Operations (cp, mv, rm, touch, find)

- **cp Command:**
  - Command: `cp filename1.txt filename2.txt`
  - Command: `cp -R /home/username/Documents /home/username/Documents_new`
- **mv Command:**
  - Command: `mv filename.txt /home/ubuntu/Documents`
  - Command: `mv old_filename.txt new_filename.txt`
- **rm Command:**
  - Command: `rm filename`
  - Command: `rm filename1 filename2 filename3`
  - Options: `-i` (interactive), `-f` (force), `-r` (recursive)
- **touch Command:**
  - Command: `touch /home/ubuntu/Documents/Web.html`
- **find Command:**
  - Command: `find /home -name notes.txt`
  - Syntax: `find [option] [path] [expression]`

![Screenshot 26-33](screenshot_26-33.png)

## Additional Command- cat, find & touch

- **cat Command:**
  - Command: `sudo cat /etc/os-release`
    - Result: Displays OS details (e.g., `PRETTY_NAME="Debian GNU/Linux 11 (bullseye)"`)
- **find Command Example:**
  - Command: `find /home -name notes.txt`
    - Result: Locates `notes.txt` in `/home` and subfolders.
- **touch Command Example:**
  - Command: `touch /home/ubuntu/Documents/Web.html1`
    - Result: Creates an empty file `Web.html1` in Document dir.

![Screenshot 34-36](screenshot_34-36.png)    
