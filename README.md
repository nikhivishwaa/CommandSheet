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
`cd "project name"`<br>
`python manage.py runserver`<br>
`python manage.py migrate`<br>
`python manage.py startapp "app name"`<br>
`python manage.py createsuperuser` superuser created in CLI<br>
`python manage.py makemigrations`<br>
`python manage.py migrate`<br>
`python manage.py shell`

## Git Commands
`git config --global user.name ""` to set name<br>
`git config --global user.email "xyz@gmail.com"` to set email<br>

View name and email by following command
`git config --global user.name` <br>
`git config --global user.name`<br>

Initilize Git Repo
`git init` initialize<br>
`ls -lart` to show hidden or .git folder in current dir<br>
`git status` to check the git project status<br>
`git add "filename"` to add file for commit<br>
`git commit -m "message or comment"` commit the change<br>
`touch "filename"` to create blank files<br>
`git add -A` to add all the files<br>
`git checkout "filename"` match this file with last commit if it commited once and now modified<br>
`git checkout -f` match all files with last commit<br>
`git log` gives all commits details<br>
`git log -p -"no. of commit fron last'` filter the commit<br>
`git diff` compare working area with staging area<br>
`git diff --staged` comparing staged file with last commit<br>
`git commit -a -m "commit message"` commit without staging the file<br>
`git rm --cached "filename"` unstage the file<br>
`git rm "filename"` delete the file from working directory<br>
`ls` list all the files<br>
`git status -s`give short status<br>
`touch .gitignore` having file name or dir which is not be tracked<br>
    `mylogs.log` ignore this file whenever it presents in dir<br>
    `/mylogs.log` ignore file in which directory .gitignore is present<br>
    `*.log` ignore the .log extension file<br>
    `folder/` ignore the entire directory<br>
`git branch "branch name"` create new branch<br>
`git checkout "branch name"` switch branch<br>
