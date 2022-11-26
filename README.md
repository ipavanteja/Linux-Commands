<h1 align="center">Linux Commands</h1>
<h2 align="center">Commands</h2>

<p align="center">
  
  Navigate to the command which you want to learn
  | [pwd](#pwd) | [cd](#cd) | [ls](#ls) | [pwd](#pwd) | [cd](#cd) | [ls](#ls) | [pwd](#pwd) | [cd](#cd) | [ls](#ls) | [ls](#ls) |
  | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
</p>

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
  **10. Type the `ls -lh` command to list the files or directories in the same table format above, but with another column representing the `size of each file/directory`.**
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

  
  
  
  
  
  
