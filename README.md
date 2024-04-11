# Git_commands

## Installation
sudo apt install git

git --version

## Connect with github account
git config --global user.name "abc123"

git config --global user.email "abc123@gmail.com"

git config --list

## clone git repository to your local system
git clone https://github.com/abc123/git_project.git

## To check any changes made in your local system
git status

#### Types of status
1. untracked -- New file is added
2. modified -- Any file is altered
3. staged -- Intermediate place before commit (Before commit file has to go through staging)
4. unmodified

## Stage changes of untracked or modfied changes
git add fine_name  ( To stage a single file)

git add .  ( To stage all file at once)
