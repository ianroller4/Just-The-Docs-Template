---
layout: default
title: The Git Life Cycle
nav_order: 2
---

<!-- prettier-ignore-start -->
# The Git Life Cycle
This page will cover the life cycle of git, the stages a file will go through in when working with git and relevant commands to the git cycle.

### Table of Contents
{: .no_toc }

1. [States of Files in The Git Life Cycle](##States-of-Files-in-The-Git-Life-Cycle)   
2. [Relevant Commands](##Relevant-Commands)  
3. [Additional Information Resources](##Additional-Information-Resources)  

{:toc}

<!--prettier-ignore-end-->


## States of Files in The Git Life Cycle
There are two possible states a file in your working directory can be, tracked or untracked. A tracked file means it was included in the latest commit within Git. A tracked file can be either unmodifed, modified, or staged.

As you edit files, Git sees them as modified, because you’ve changed them since your last commit. As you work, you selectively stage these modified files and then commit all those staged changes, and the cycle repeats.

__The four stages of a file are:__

- __Untracked__

A file is in your working directory but not within your last commit.

- __Unmodified__

A tracked file that was within your last commit and hasn't been changed.

- __Modified__

A tracked file that was within your last commit and has been modified but not staged yet, and thus isn't able to be commited.

- __Staged__

An untracked or modified file that has been staged is ready to be commited to the repo.

## Relevant Commands
__Show Status:__ To check the status of the working directory for changes or additions, use:

```console
git status
```
__Stage Files:__ To stage a specific file, use: 
```console
git add <file-name>
```
To stage all unstaged files within your working directory, use:
```console
git add .
```
__Commiting Changes:__ To commit staged files to the repo, use:
```console
git commit -m "Commit Message"
```

__Show Differences__: To show the differences between your current working directory and the last commit made, use:
```console
git diff
```


## Additional Information Resources
- [Toolsqa - Git Life Cycle](https://www.toolsqa.com/git/git-life-cycle)
- [Git Basics - Recording Changes to the Repository](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)
- [Geeks for Geeks - Git Life Cycle](https://www.geeksforgeeks.org/git/git-life-cycle)

