# Existing-repository
How to use Git and Github on a non empty folder on the local computer and syncronize it with Github.
Important! Use Git Bash to execute Git commands on the local computer.
# Create a local repository on the computer
## Change to the folder on the local computer containing the project files.
```
Important! The file path separator in Git Bash is "\" instead of "/" in Windows. Example:
C:\users\username\Desktop\Excisting repository
becomes:
/c/Users/username/Desktop/Excisting repository
Git Command:
$ cd "/c/Users/username/Desktop/Excisting repository"
```
## Create local repository
```
Git Command:
$ git init
```
## Add all files from the folder to the repository
```
Git Command:
$ git add -A
```
## Initial commit of all files 
```
Git Command:
$ git commit -m "Initial commit of the project", remember a comment at each commit
```
# Create remote repository on Github
Log on to Github
Click on: New
Fill out Repository name
Important! You can give the remote repository any name, but it is a good idea to choose a name similar to the local repository
Choose: Public
Important! The project has to be public for the initial push from the local repository
Very important! DO NOT CHOOSE TO ADD A README FILE! If you do, the following git remote will fail. Add the readme later. This is because the remote readme file is not in the local repository!
Optional: Choose GitIgnore
Optional: Choose Licence
# Syncronise local repository with remote repository
## Make a link
```
Git Command:
$ git remote add origin https://github.com/username/remote-repository-name.git
```
## Initial push of the project
```
Git Command:
$ git push -u origin master
```
The local and the remote repository are now synchronized and ready for daily operations.
Ad the following sections to any readme-file:
# Local repository
```
$ cd "/c/Users/username/Desktop/Excisting repository"
```
# Working on a daily basis
## Pull from the remote repository to the local repository
Do this before work begins in the local repository
```
$ git pull
```
## Push files from the local repository to the remote repository
Do this on a regular basis during work
```
Add files and changes to files
Git command:
$ git add -A
Commit changes to local repository
Git command:
git commit -m "Comment", remember a comment at each commit
Push from the local repository to the remote repository
$ git push

