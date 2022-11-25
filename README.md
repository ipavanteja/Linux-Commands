<h1 align="center">Linux Commands</h1>

- ## pwd

  `pwd` stands for **Print Working Director**.<br/>
  It prints the full pathname of the current working directory starting from the root.
  ### Syntax:
  ```
  $ pwd
  ```
  #### Example:
  ```
  teja@LAPTOP:Users/Teja$ pwd
  Users/Teja
  ```
- ## cd
  
  `cd` stands for **Change Directory**.<br/>
  Used to change the current working directory. We can move all over our directories in our system.<br/>
  
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
  - We can use single quotes insted of double quotes, `cd 'App Data'`
  
  
  
  
  
  
  
  
  
  
  
  
  
  
