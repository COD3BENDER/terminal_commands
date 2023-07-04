# **Terminal Commands and Git Cheat Sheet**

## *Terminal Commands*

<br><br/>

| Commands    | Description |
| ----------- | ----------- |
| `pwd` | Displays the location in the terminal you are currently in with the path to it. |
| `cp` | Used to copy files (To copy directories you have to add the -r flag, so `cp -r` - this will loop the command until all items in the directory is copied.)<br> **Example:** `cp example_c.txt ~/Desktop` <br/>|
| `mv` | Used to move files or directories ( you need to specify the directory you want to move the file to.) <br> **Example:** `mv example_m.txt ~/Desktop`) <br/>|
| `ls` | this will list all the files and directories you can navigate to from the working directory.|
| `ls -a` | Similar to `ls` but the `-a` flag means all and will also show hidden files/directories |
| `cd folder` | Is used to navigate directories and change the working directory. <br> **Example:** `cd Desktop` will take you to desktop <br/> |  |
| `cd ..` | Will take you back one directory |
| `cd`  | Will take you to the root directory |
| `code .`  | Will open the current folder in vscode|
| `code file.txt`  | Will open file.txt in vscode|
| `rm` | rm is used to remove files|
| `rm -r`| used to remove directories|
| `rm -rf`| forcefully remove directories/files even if they are protected|
| `mkdir name`| to make a directory|
| `touch name.txt`| used to make files if there isnt and update files if there is can change the file extension .txt, .java, .py ...|


<br><br/>

## *Git Commands*

<br><br/>

**IMPORTANT** - *Especially when collaborating* -  when you want to push you work try to first pull the latest version before you push your work otherwise it can corrupt the files.

When inside the folder you want to track with git run the command below to initialize git.
```
git init
```
it will change the terminal to:
```
>> folder_name git:(main)
```
when you create a file within the folder it will be untracked so you must add the tracking to that file using the command below:
```
git add filename.txt
or git add . (to add all files in the directory)
```
after you added the changes you can commit the changes but you must also add a message as done below
```
git commit -m "add relevant message"
```
To check the status of your repository use command:
```
git status
```
To see the commit history you can use the command:
```
git log
```
To roll back changes and keep history use the command (you can find the ID you want to roll back to using git log):
```
git revert IDxxxx 
```

to link local repository to GitHub repository use:
```
git remote add origin url
```
to pull from version control:
```
git pull
or git pull origin main
```
to push to GitHub:
```
git push origin main
```
*you can also push to a different branch if you have 

to clone a repository:
``` 
git clone url
``` 

.gitignore files are used to make git ingnore files for tracking such as the .venv folder when using intellij you can specifiy in your .gitignore files what file or types of files you dont want tracked and they wont get pushed.



