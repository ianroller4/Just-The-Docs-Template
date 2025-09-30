# Git Fundamentals

Git is a distributed version control system that allows developers to track changes in their code, collaborate with others, and maintain a history of their projects. This page covers the essential fundamentals of Git.

## Table of Contents
- [Configuring Git](#configuring-git)
- [Initializing a Repo](#initializing-a-repo)
- [Staging and Commit Files](#staging-and-commit-files)
- [Status, Log, and Diff](#status-log-and-diff)
- [Working with Branches](#working-with-branches)
- [Remotes and Pushing](#remotes-and-pushing)
- [Using a Git Ignore File](#using-a-git-ignore-file)
- [Summary](#summary)
- [Learn More](#learn-more)

---

## Configuring Git

Before using Git, you need to configure your identity and preferences.

**Commands:**
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
```
The --global flag applies the settings to all repositories for the current user.
To set configuration only for the repository you are currently in, omit the --global flag.

## Initializing a Repo 

A repository (repo) is where Git stores your project history.

**Commands:**

```bash
git init
git clone <repository_url>
```
git init turns an existing directory into a Git repository by creating a .git folder.

git clone copies a remote repository to your local machine and sets up origin as the default remote.

## Staging and Commit Files
Git tracks changes through a two-step process: staging and committing.

**Commands:**

```bash
git add filename.txt
git add .
git commit -m "Describe what changed"
```
You can add specific files or file types

git add . adds all unstaged files

Staging prepares changes to be committed.

Commit saves the staged snapshot into the repository history.

## Status, Log, and Diff
Useful commands to inspect repository state and history:

```bash
git status
git log
git log --oneline
git diff
git diff --staged
git status 
```
git log shows commit history. Options like --oneline, --graph, and --decorate give a more compact view.

git diff shows changes in files that have not yet been committed.

git status shows unstaged, staged, and untracked files. Also tells you what branch you are working in.

## Working with Branches
```bash
git checkout main
git checkout -b feature/awesome
git branch
git merge feature/awesome
git branch -d feature/awesome
```
Branches let you work on separate lines of development.

git checkout takes your current unstaged files and brings them to a different branch

adding -b to checkout creates a new branch

Merging brings changes together.

Rebasing can be used for a linear history.

## Remotes and Pushing
```bash
git remote -v
git remote add origin git@github.com:me/repo.git
git push -u origin main
git pull
```
Remotes let you share your repository with others.

git remote -v gives info on the remote repo

git remote add connects a remote repo to your repo

git push sends your latest commit to the remote repo in order to make a pull request

The -u flag sets upstream so you can use git push and git pull without specifying remote and branch.

git pull grabs the latest changes to the remote repo and applies them to your local one

## Using a .gitignore File
The .gitignore file tells Git which files and directories to ignore. It can be edited like a .txt file and every line is a file that git will ignore.
You can tell it to ignore entire folders, all files of a type (.txt, .log, etc), or specific files

Example:

```bash
node_modules/ (This would ignore an entire folder named node_modules)
*.log	(This would ignore all files with the extension .log)
New Text.txt  (This would ignore only a text file named New Text)
node_modules/*.log  (This would ignore all .log files in the node_modules folder)
```
This prevents unwanted files (build outputs, OS-specific files) from being tracked.

Tracked files must be removed with git rm --cached to actually be ignored afterward.

## Summary

Configure Git with your name and email (git config).

Initialize or clone repositories (git init, git clone).

Stage changes with git add, commit them with git commit.

Inspect state with git status, git log, and git diff.

Manage branches with git branch, git checkout -b, git merge, git branch -d.

Work with remotes using git remote -v, git push, git pull, git fetch.

Undo mistakes with git restore, git reset, git revert.

View differences and history with git log --oneline --graph --decorate.

Use .gitignore to exclude unnecessary files.

## Learn More
- [Official Git Documentation](https://git-scm.com/doc)  
- [Pro Git Book (free online)](https://git-scm.com/book/en/v2)  
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)  
- [GitHub Docs](https://docs.github.com/en/get-started/using-git)  
- [Git Cheatsheet (PDF)](https://training.github.com/downloads/github-git-cheat-sheet.pdf)  