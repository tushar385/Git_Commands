# Git Commands

## Installation
sudo apt install git

git --version

## Connect with github account
git config --global user.name "abc123"

git config --global user.email "abc123@gmail.com"

git config --list

## clone git repository to your local system
git clone https://github.com/abc123/git_project.git

## Clone specific branch to local system
git clone -b branch1 https://github.com/abc123/git_project.git


------------------------------------------------------------------------------------------------------------------
# Git add, commit, push command

## To check any changes made in your local system
git status

#### Types of status
1. untracked -- New file is added
2. modified -- Any file is altered
3. staged -- Intermediate place before commit (Before commit file has to go through staging)
4. unmodified

## Stage changes of untracked or modfied changes
git add file_name  ( To stage a single file)

git add .  ( To stage all file at once)

## Commit changes of stageing
git commit -m "message" ( by commit chnages will not reflect in github UI, so also have to push)

## Push 
git push origin main

------------------------------------------------------------------------------------------------------------------
# Git Initialization commands

## To check if the current folder is a git connected folder or not
ls -a  (it will have a .git file)

## To initialize current folder as a git folder
git init

## To connect cwd with github repository
git remote add origin https://github.com/abc123/git_project2.git

## To delete cwd connection with github repository
git remote rm origin

## To verify cwd is connected to which github repository
git remote -v

------------------------------------------------------------------------------------------------------------------
# Git commands for working with branches

## Check current branch name
git branch

## Rename Branch
git branch -M tushar_branch

## Make new branch
git checkout -b tushar_branch2

## To switch between branch
git checkout tushar_branch

## To check code difference between 2 branches
git diff tushar_branch

## To merge current branch with other branch (add other branch code in current branch)
git merge tushar_branch2

## To pull changes made by other in github on your branch (streamline changes of others code in your local system)
git pull origin tushar_branch

------------------------------------------------------------------------------------------------------------------
# Git rollback commands

## logs
git log

# Undoing changes

## Staged changes ( when we do git add .)
git reset file_name  ( To reset a single file)

git reset ( To reset a all file)

## commited changes ( when we do git commit -m 'message'
git reset Head~1

## commited changes ( rollback to multiple commit's)
git reset commit_hash  (hash code to be obtained from git log)

git reset --hard commit_hash ( to rollback commit & rollback code in vs code also)
