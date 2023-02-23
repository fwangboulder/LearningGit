
# What does Git do?

1. Manage projects with Repositories
2. Clone a project to work on a local copy
3. Control and track changes with Staging and Committing
4. Branch and Merge to allow for work on different parts and versions of a project
5. Pull the latest version of the project to a local copy
6. Push local updates to the main project

# Working with Git

1. Initialize Git on a folder, making it a Repository
2. Git now creates a hidden folder to keep track of changes in that folder
3. When a file is changed, added or deleted, it is considered modified
4. You select the modified files you want to Stage
5. The Staged files are Committed, which prompts Git to store a permanent snapshot of the files
6. Git allows you to see the full history of every commit.
7. You can revert back to any previous commit.
8. Git does not store a separate copy of every file in every commit, but keeps track of changes made in each commit!

## [git cheat sheet](https://training.github.com/downloads/zh_CN/github-git-cheat-sheet/)

## [Work with multiple github accounts](https://gist.github.com/fwangboulder/26be6aaea0359196e29989169a5792cd)
```
1. Git install:
download Git for free from the following website: https://www.git-scm.com/

git --version

2. Configure git

git config --global user.name "name"
git config --global user.email "email"

3. Creating Git folder

mkdir myproject
cd myproject

4. Initialize git
git init

git status
git add filename
git add --all
git commit -m "commit message"
git status --short
??, A, M, D (untracked, added, Modified, Deleted)
git commit -a -m "message"

git log
git commit -help
git help --all

git branch branchname
git branch
git checkout branchname
git status
git checkout master
git checkout -b emergency-fix

git checkout master
git merge emergency-fix
git branch -d emergency-fix
(merge the branch and delete it)

git checkout branchname
git add --all
git commit -m "message"
git checkout master
git merge branchname
git status
git add filename
git status
git commit -m "merged"
git branch -d branchname

git pull
git status
git branch
git branch -a
```
## Important
1. git commit saves repository changes on local but not remote repository.
Contrarily, Git push then updates your git commit changes and sends it to
remote repository.
2. The git pull command is used to fetch and download content from a remote
repository and immediately update the local repository to match that content.
3. Git fetch is a primary command used to download contents from
  a remote repository. Git fetch + git merge = git pull
4. Git clone: Cloning an Existing Repository.
Every version of every file for the history of the project is pulled down by
 default when you run git clone .
