-----------------------------------------------------------------------------------------------------------------------------

#configuration of git

git config --global user.name "dipaktamang"--------->which indicate the username of workplace 

git config --global user.email "dt1414926@gmail.com"--->which indicates the useremail of workplace

git config --gif----->this command show the all the configuration

-----------------------------------------------------------------------------------------------------------------------------

#clone & status

git clone ---some link----->cloning the repo on our local machine

git status --->display the state of the code

ADD + COMMIT------->process of upgrate code

    TYPES OF STATUS
      untracted-------->NEW FILE GIT DOESN'T TRACK YET
          |
      modified--------->CHANGED
          |
        staged--------->FILE IS READY TO BE COMMITED
          |
       unmodified------>UNCHANGED

-----------------------------------------------------------------------------------------------------------------------------

ls -a ----->show a hidden file in repo

-----------------------------------------------------------------------------------------------------------------------------

#ADD & COMMIT

ADD---------->adds new or changed file in your working directory to the git staging area.

git add <file name>

git add . ---->It is used for add all of the changes

COMMIT------->it is the record of change

git commit -m <message>

-----------------------------------------------------------------------------------------------------------------------------

#PUSH COMMAND
PUSH-------->upload local repo to remote repo
git push origin main

-----------------------------------------------------------------------------------------------------------------------------

#COMMAND INIT

INIT----->used to create a new repo

git init---------->initialized the repo

git remote add origin <link>------>it changes the location of the code to another repo

git remote -v -------->to verify remote,find the state of repo

git remote set-url origin <link of repo>

git branch ---->To check branch

git branch -M main----->To rename branch

git push origin main

git push -u origin main-------->there no need to enter orgin/branches

-----------------------------------------------------------------------------------------------------------------------------

                    #WORKFLOW#                                       #REMOTE PUSH#
                -------------------                            ------------------------
                  git hube repo                                       git init
                        |                                                |
                      clone                                git remote add origin <link of repo>
                        |                                                |
                     changes                                         git remote -v
                        |                                                |
                      commit                               git remote set-url origin <link of repo>
                        |                                                |
                       push                                     git checkout -b main
                                                                         |
                                                                  add ,commit ,push
                                                              

-----------------------------------------------------------------------------------------------------------------------------

#GIT BRANCHES

git branch------------------>To check branch

git branch -M main------------->Reaneme branch

git checkout <branchname>--------->To navigate

git checkout -b <new branchname>----->To create a new branch

git branch -d <branchname>-------------->to delete branch

-----------------------------------------------------------------------------------------------------------------------------

                                      #MERGING CODE#
                      
                                         WAY 1
                                     --------------
                                 git diff <branch name>
                                 git merge <branch name>
                                 
                                         WAY 2
                                    ---------------
                                 create a PR(pull request)

-----------------------------------------------------------------------------------------------------------------------------

#PULL REQUEST

It lets you tell others about changes you've pushed to a branch in a repository on Github.

-----------------------------------------------------------------------------------------------------------------------------

#PULL COMMAND#

git pull origin main

used to fetch and download content from a remote repo and immediately update the local repo to match that content

-----------------------------------------------------------------------------------------------------------------------------

#RESOLVING OF MERGE COMFLICT #

An event that takes place when git is unable to automatically resolve differences in ocde between two commits.

-----------------------------------------------------------------------------------------------------------------------------

#Undoing Changes

Case 1:staged changes------availe for commit stage

   git rset <file name>
   
   git reset
   
Case 2:Commited changes(for one commit)

git reset HEAD~1

Case 3:Commited changes(for many commits)

git reset <commit hash>-------------->only chnage the commit

git reset --hard <commit hash>---------->change the commited code in vscode

-----------------------------------------------------------------------------------------------------------------------------

#Fork

A for is a new repo that shares code and visibility setting with the original "upstream" repository.
Fork is a rough copy.
