# GIT
* Global Information Tracking System
### Repository
* it is just like folder with some extra capabulityes 
* it is a folder haveing some storage
### stages in git hub
1. workspace
2. stageing area (temparary area (add))
3. local repo (commit)
4. central repo (push)
#### git commands
* to inisialise a folder as git repo
    * **git init**
* we known that what is the status of our file
    * **git status**
* temparary area  it is storeing area
    * **git add file_name** to add particular file
    * **git add .** to add all files
* to change the existing branch 
    * **git branch**    to see existing branches
    * **git branch -M branch_name**  to create a new branch we genrally give main

* to commit the files with message it is nothing but local repo
    * **git commit -m "write a message"**
* **to do commit we have to set configureation**
    * **git config --global user.name "user_name"**
    * **git config --global user.email "email_id"**
* before pushing to central repo give the link where we have to push has shown below
    * **git remote add orgin url"**
    * url can be http or git url
* pushing the changes to central repo
    * **git push orgin branch_name**
* to perform all command at once use semi colon as shown below
    * **git add .; git commit -m "first commit"; git push orgin main**
* To get all the folders we have in the git hub to a instance use below command 
    * **git clone url**
* to add newly added script to instace use below command 
    * **git pull**
* if you want to edit existing user_name and email
    * **git config --global --unset -all user.name**
    * **git config --global --unset -all user.email**
* if you want to add existing remote orgin
    * **git remote set-ur orgin new_url"**
* to see all the commit history in git hub use below command below
    * **git log**
* reverse incremental search
    * press **ctrl + r** type a unique key word in command continue pressing **ctrl + r** 
* grep git
      * **history | grep "type what-you-want-to-search"**
* whwn two commands are running simultaniusly in git  use below command
    *  **rm -f .git/index.lock**
* to remove file from git repository from github
      * **git rm file_name; git commit -m "first commit"; git push orgin main**
* to remove a git repository from github
      * **git rm --cached repository_name; git commit -m "first commit"; git push orgin main**