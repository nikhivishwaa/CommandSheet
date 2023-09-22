# CommandSheet
This is Sheet For Commands
## Powershell
Script execution Policy `Enable/Disable` 
* <h5><i></i>Run following command in Windows Powershell ISE</i></h5> 
```Set-ExecutionPolicy RemoteSigned -Scope CurrentUser```

## Virtual ENV
 `Enable/Disable` ok go

`pip freeze > requirements.txt`

 `pip install -r requirements.txt`

## Django Commands
`django-admin startproject "Project name"`<br>
`cd "project name"`
`python manage.py runserver`
`python manage.py migrate`
`python manage.py startapp "app name"`
`python manage.py createsuperuser` superuser created in CLI
`python manage.py makemigrations`
`python manage.py migrate`
`python manage.py shell`

## Git Commands
`git config --global user.name ""` to set name
`git config --global user.email "xyz@gmail.com"` to set email

View name and email by following command
`git config --global user.name` 
`git config --global user.name`

Initilize Git Repo
`git init` initialize
`ls -lart` to show hidden or .git folder in current dir
`git status` to check the git project status
`git add "filename"` to add file for commit
`git commit -m "message or comment"` commit the change
`touch "filename"` to create blank files
`git add -A` to add all the files
`git checkout "filename"` match this file with last commit if it commited once and now modified
`git checkout -f` match all files with last commit
`git log` gives all commits details
`git log -p -"no. of commit fron last'` filter the commit
`git diff` compare working area with staging area
`git diff --staged` comparing staged file with last commit
`git commit -a -m "commit message"` commit without staging the file
`git rm --cached "filename"` unstage the file
`git rm "filename"` delete the file from working directory
`ls` list all the files
`git status -s`give short status
`touch .gitignore` having file name or dir which is not be tracked
    `mylogs.log` ignore this file whenever it presents in dir
    `/mylogs.log` ignore file in which directory .gitignore is present
    `*.log` ignore the .log extension file
    `folder/` ignore the entire directory
`git branch "branch name"` create new branch
`git checkout "branch name"` switch branch
