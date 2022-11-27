<h1 align="center">Linux Commands</h1>

[Linux](https://www.linux.org/) is a open-source Unix operating systems based on the Linux Kernel. The Linux commands are useful for operating the Linux operating system. All basic and advanced tasks can be done by executing commands. The commands are executed on the Linux terminal, It’s similar to the Command Prompt application in Windows. Keep in mind that all Linux commands are case-sensitive. 

<h2 align="center">Commands</h2>
  
  Navigate to the command that you want to learn
  | [pwd](#pwd) | [cd](#cd) | [ls](#ls) | [mkdir](#mkdir) | [rm](#rm) | [rmdir](#rmdir) | [pwd](#pwd) | [cd](#cd) | [ls](#ls) | [ls](#ls) |
  | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |

- ## pwd

  - `pwd` stands for **Print Working Director**.<br/>
  - It prints the full pathname of the current working directory starting from the root.
  ### Syntax:
  ```
  $ pwd
  ```
  #### Example:
  ```
  teja@LAPTOP:Users/Teja$ pwd
  Users/Teja
  ```
  [⬆ Go to Top](#commands)
- ## cd
  
  - `cd` stands for **Change Directory**.<br/>
  - Used to change the current working directory. We can move all over our directories in our system.<br/>
  
   **1. To navigate to a directory from root directory -**
  ```
  $ cd [/Root_Name/Destination_Path]
  ```
  ```
  teja@LAPTOP:/mnt/c$ cd /mnt/c/Users/Teja
  teja@LAPTOP:/mnt/c/Users/Teja$
  ```
  **2. To navigate to next directory(sub directory) -**
  ```
  $ cd [SubDirectory_Name]
  ```
    ```
    teja@LAPTOP:Users/Teja$ cd Desktop
    teja@LAPTOP:Users/Teja/Desktop$
    ```
  **3. To navigate to previous directory(parent directory of current directory) -**
  ```
  $ cd ..
  ```
  ```
  teja@LAPTOP:Users/Teja/Desktop$ cd ..
  teja@LAPTOP:Users/Teja$
  ```
  **4. To navigate to root directory -**<br/>
  - The root directory is the first directory in our filesystem.
  ```
  $ cd /
  ```
  ```
  teja@LAPTOP:Users/Teja/Desktop$ cd /
  teja@LAPTOP:/$
  ```
  **5. To navigate to home directory -**
  ```
  $ cd ~
  ```
  ```
  teja@LAPTOP:Users/Teja/Desktop$ cd ~
  teja@LAPTOP:~$
  ```
  ```
  $ cd
  ```
  - This above command is also work as `cd ~` <br/>
  
  **6. To navigate to a directory with spaces in directory name -**
  ```
  $ cd ["Dictory_Name"]
  ```
  ```
  teja@LAPTOP:Users/Teja$ cd "App Data"
  teja@LAPTOP:Users/Teja/App Data$
  ```
  - We can use single quotes insted of double quotes, `cd 'App Data'`<br/>
  
  [⬆ Go to Top](#commands)
- ## ls
  - `ls` command is known for list files or directories which are present in a directory.<br/>
  ### Syntax:
  ```
  $ ls
  ```
  #### Example:
  
  **1. List files or content in the present working directory -**
  ```
  teja@LAPTOP:Users/Teja$ ls
  Desktop       Music       Games
  Documents     Picturies   Videos
  Downloads   
  ```
  **2. List files in the another working directory -**
  
  ### Syntax:
  ``` 
  $ls [Directory_Name] 
  ```
  ```
  teja@LAPTOP:Users/Teja$ ls Desktop
  Brave.lnk  'Microsoft Edge.lnk'  'Sublime Text.lnk'  'Visual Studio Code.lnk'
  ```
  **3. Type the `ls /` command to list the contents of the `root directory`.**<br/>
  **4. Type the `ls ..` command to list the contents of the `parent directory` one level above. Use `ls ../..` for contents two levels above.**<br/>
  **5. Type the `ls ~` command to list the contents in the users's `home directory`.**<br/>
  **6. Type the `ls -d */` command to list `only directories`.**<br/>
  **7. Type the `ls *` command to list the contents of the `directory` with it's `subdirectories`.**<br/>
  **8. Type the `ls -s` command (the s is lowercase) to list files or directories with their `sizes`.**<br/>
  **9. Type the `ls -l` command to list the contents of the directory in a `table format` with `columns including`.**<br/>
  ```
  teja@LAPTOP:Users/Teja$ ls -l
  drwxrwxrwx 1 teja teja    4096 Nov 25 14:51  Desktop
  drwxrwxrwx 1 teja teja    4096 Nov 25 18:39  Documents
  drwxrwxrwx 1 teja teja    4096 Nov 25 20:39  Downloads
  drwxrwxrwx 1 teja teja    4096 Nov 27  2021  Music
  drwxrwxrwx 1 teja teja    4096 Oct 28 20:02  Pictures
  drwxrwxrwx 1 teja teja    4096 Nov 27  2021  Games
  drwxrwxrwx 1 teja teja    4096 Nov 19 22:24  Videos
  ```
  **10. Type the `ls -lh` command to list the files or directories in the same table format above, but with another column representing the `size of each
  file/directory`.**
  ```
  teja@LAPTOP:Users/Teja$ ls -lh
  drwxrwxrwx 1 teja teja 4.0K Nov 25 14:51  Desktop
  drwxrwxrwx 1 teja teja 4.0K Nov 25 18:39  Documents
  drwxrwxrwx 1 teja teja 4.0K Nov 25 20:39  Downloads
  drwxrwxrwx 1 teja teja 4.0K Nov 27  2021  Music
  drwxrwxrwx 1 teja teja 4.0K Oct 28 20:02  Pictures
  drwxrwxrwx 1 teja teja 4.0K Nov 27  2021  Games
  drwxrwxrwx 1 teja teja 4.0K Nov 19 22:24  Videos
  ```
  **11. Type the `ls -a` command to list files or directories including `hidden files or directories`. In Linux, anything that begins with a `.`is considered a `hidden   file`**<br/>
  ```
  teja@LAPTOP:Users/Teja$ ls -a
  .bash_history        Desktop      Music       Games
  .gitconfig           Documents    Pictures    Videos
  .lesshst             Downloads
  .minttyrc            
  .node_repl_history
  ```
  **12. Type the `ls -t` command to list files or directories and sort by `last modified date` in descending order (biggest to smallest).**<br/>
    - You can also add a `-r` flag to reverse the sorting order like so: `ls -tr`<br/>
    
  **13. Type the `ls -S` (the S is uppercase) command to list files or directories and sort by `size in descending order` (biggest to smallest).**<br/>
    - You can also add a `-r` flag to reverse the sorting order like so: `ls -Sr`<br/>
    
  **14. Type the `ls > [File_Name].txt` command to print the output of the preceding command into an `File_Name.txt` file.**<br/>
    - You can use the file as you see fit, or log the contents of the file with `cat File_Name.txt`<br/>
  ```
  teja@LAPTOP:Users/Teja$ ls > file.txt
  teja@LAPTOP:Users/Teja$ cat file.txt
  Desktop
  Music
  Games
  Documents
  Picturies
  Videos
  Downloads
  ```
  [⬆ Go to Top](#commands)

- ## mkdir
  - mkdir command is used to create new directories.<br/>
  - This command can create multiple directories at once as well as set the permissions for the directories.<br/>
  ### Syntax:
  ```
  $ mkdir [Directory_Name]
  ```
  #### Example:
  ```
  teja@LAPTOP:Users/Teja/Games$ ls
  Action
  teja@LAPTOP:Users/Teja/Games$ mkdir Adventure
  teja@LAPTOP:Users/Teja/Games$ ls
  Action     Adventure
  ```
  - `-v` flag will prints a message for each created directory.
  ```
  $ mkdir -v [Directory_Name]
  ```
  - We can create multiple directories at a time by `mkdir [Dir1] [Dir2] [Dir3]`
  - We can create sub-directories also by using `-p` flag.
  ```
  $ mkdir -p [dir1_nanme/dir2_name/dir3_name]
  ```
  
  ```
  teja@LAPTOP:Users/Teja$ mkdir -p dir1/dir2/dir3
  teja@LAPTOP:Users/Teja$ ls
  dir1
  teja@LAPTOP:Users/Teja$ cd dir1
  teja@LAPTOP:Users/Teja/dir1$ ls
  dir2
  teja@LAPTOP:Users/Teja/dir1$ cd dir2
  teja@LAPTOP:Users/Teja/dir1/dir2$ ls
  dir3
  ```
  - `-m` sets the file permissions. For instance, to create a directory with full read, write, and execute permissions for all users.
  ```
  $ mkdir -m777 [directory_name]
  ```
  [⬆ Go to Top](#commands)
  
- ## rm
  - `rm` command is used to delete files and folders(directories).
  ### Syntax:
  ```
  $ rm [File or Directory]
  ```
  #### Example:
  ```
  teja@LAPTOP:Users/Teja$ ls
  file1.txt      file2.txt     file3.txt
  teja@LAPTOP:Users/Teja$ rm file1.txt
  teja@LAPTOP:Users/Teja$ ls
  file2.txt     file3.txt
  ```
  - `-i` option makes the command ask the user for confirmation before removing each file. `rm -i file1.txt`.
  - `-f` (force deletion) option overrides `write protected` and removes the file forcefully.
  - We can delete multiple files at a time by `rm file1.txt file2.txt file3.txt`.
  - Deleting directories -
  - `-d` option will remove empty directories.
  ```
  $ rm -d [Directory_Name]
  ```
  - `-d` option can't delete non-empty directories.
  - `-r` option removes all the files and sub-directories (non-empty directories) in the parent directory.
  ```
  teja@LAPTOP:Users/Teja$ ls
  Desktop       Music       Games
  teja@LAPTOP:Users/Teja$ rm -r Games
  teja@LAPTOP:Users/Teja$ ls
  Desktop       Music
  ```
  [⬆ Go to Top](#commands)
  
- ## rmdir
  - `rmdir` command is used to delete an empty directory permanently.
  ### Syntax:
  ```
  $ rmdir [Directory_Name]
  ```
  #### Example:
  ```
  teja@LAPTOP:Users/Teja$ ls
  Desktop       Music       Games
  teja@LAPTOP:Users/Teja$ rmdir Games
  teja@LAPTOP:Users/Teja$ ls
  Desktop       Music
  ```
  - `rmdir` can't delete a directory if it's not empty. For that we have to use [rm -r](#rm) command.
  - `-p` works for deleting a subdirectory and its parent directory.
  ```
  $ rmdir -p /Directory/SubDirectory
  ```
  - `-v` option will print a text as a confirmation that the specified directory has been deleted.
  
  [⬆ Go to Top](#commands)

- ## touch
   - `touch` command is used to create empty files, change modify the timestamps of files or folders.
   ### Syntax:
   ```
   $ touch [File_Name]
   ```
   #### Example:
   ```
   teja@LAPTOP:Users/Teja$ ls
   teja@LAPTOP:Users/Teja$ touch file.txt
   teja@LAPTOP:Users/Teja$ ls
   file.txt
   ```
   - We can create `multiple files` at a time by `touch file1.txt file2.txt file3.txt`.
   - You can `auto generate file` names using curl braces while creating multiple files like in the following example:
   ```
   $ touch file_name{1..3}.txt
   $ ls
   file_name1.txt    file_name2.txt    file_name3.txt
   ```
   - `-a` option will change the `access time` of a file to the current time.
   ```
   $ stat file.txt
   Access: (0777/-rwxrwxrwx)  Uid: ( 1000/    teja)   Gid: ( 1000/    teja)
   Access: 2022-11-27 16:55:19.142152800 +0530
   Modify: 2022-11-27 16:53:31.937936000 +0530
   Change: 2022-11-27 16:55:18.013885600 +0530
   $ touch -a file.txt
   Access: (0777/-rwxrwxrwx)  Uid: ( 1000/    teja)   Gid: ( 1000/    teja)
   Access: 2022-11-27 17:00:19.142152800 +0530
   Modify: 2022-11-27 16:53:31.937936000 +0530
   Change: 2022-11-27 17:00:18.013885600 +0530
   ```
   - `-m` option will change the `modification time only`. This will update last modification time.
   ```
   $ touch -m [File_Name]
   ```
   ```
   $ stat file.txt
   Access: (0777/-rwxrwxrwx)  Uid: ( 1000/    teja)   Gid: ( 1000/    teja)
   Access: 2022-11-27 17:00:19.142152800 +0530
   Modify: 2022-11-27 16:53:31.937936000 +0530
   Change: 2022-11-27 17:00:18.013885600 +0530
   
   $ touch -m file.txt
   Access: (0777/-rwxrwxrwx)  Uid: ( 1000/    teja)   Gid: ( 1000/    teja)
   Access: 2022-11-27 17:15:25.142152800 +0530
   Modify: 2022-11-27 17:15:25.937936000 +0530
   Change: 2022-11-27 17:15:25.013885600 +0530
   ```
   - `-am` option will change the both `access time` and `modification time`.
   - 
  
  
  
  
