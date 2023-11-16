# CommandSheet
This is Sheet For Commands
## Powershell
Script execution Policy `Enable/Disable` 
* <h5><i></i>Run following command in Windows Powershell ISE</i></h5> 
```Set-ExecutionPolicy RemoteSigned -Scope CurrentUser```

## Virtual ENV
`python -m venv "project1"` create new environment

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
`python manage.py shell`<br>
    `from models import "class"`
    `class.objects.all()` list all objects of query class
    `class.objects.get(parameter='xyz')` get specific objects of query class
    `a = class.objects.get(parameter='xyz')` 
    `a.attributes` access object
`go to admins.py then write following code` Register models <br>
`from .models import "table class"`<br>
`admin.site.register("table class")`<br>

## Git Commands
`git config --global user.name ""` to set name<br>
`git config --global user.email "xyz@gmail.com"` to set email<br>

View name and email by following command<br>
`git config --global user.name` <br>
`git config --global user.name`<br>

Initilize Git Repo<br>
`git init` initialize<br>
`code .` open editor<br>
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
`git merge` merge new branch to master<br>
`git branch` list all the branches<br>
`git checkout -b "branch name"` create a new branch and switch on it<br>
`git branch -d "branch name"` delete a branch from local area<br>
`git branch -D "branch name"` delete a branch which is commited once local area<br>
`git remote add "origin" "repo url".git` add remote repository<br>
`git remote` check the origin name list<br>
`git remote -v` fetch and push url<br>
`git push "origin" "branch name"` push code on github<br>
`ssh-keygen -t rsa -b 4096 -C "name@email.com"` generate ssh key<br>
`eval $(ssh-agent -s)` deploy ssh key<br>
`ssh-add ~/.ssh/id_rsa` add ssh<br>
`cat ~/.ssh/id_rsa.pub` see long ssh key<br>
`git remote set-url "existing origin" "ssh url"`<br>
`git push -u "origin" "branchname"` push code to github repo in specified branch<br> 
`git clone "repo-url"` clone repository in repo-url folder<br>
`git clone "repo-url" "repo-1"` clone repository in repo-1 folder<br>
