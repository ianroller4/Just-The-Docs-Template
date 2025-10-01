---
layout: default
title: Creating, Using, and Merging Branches
nav_order: 5
---

# Git Branching Guide

Git branches are a powerful feature that allow developers to work on separate lines of development without interfering with the main project. Branching makes it easier to experiment, fix bugs, and collaborate on new features.

---

## Table of Contents
1. [Introduction to Branches](#introduction-to-branches)  
2. [Creating a Branch](#creating-a-branch)  
3. [Switching Between Branches](#switching-between-branches)  
4. [Merging Branches](#merging-branches)  
5. [Deleting Branches](#deleting-branches)  
6. [Summary](#summary)  
7. [Learn More](#learn-more)  

---

## Introduction to Branches
A branch in Git is a lightweight movable pointer to a commit. The default branch name is usually `main` or `master`. Branches let you develop features, test changes, and work independently before merging them back into the main project.

---

## Creating a Branch
You can create a new branch from the current commit using:

```bash
git branch <branch-name>
```

To create and immediately switch to a new branch:

```bash
git checkout -b <branch-name>
```

---

## Switching Between Branches
To move between branches, use:

```bash
git checkout <branch-name>
```

Or with the newer command:

```bash
git switch <branch-name>
```

---

## Merging Branches
To combine changes from one branch into another:

1. Switch to the branch you want to merge **into** (often `main`):
   ```bash
   git checkout main
   ```
2. Merge the target branch:
   ```bash
   git merge <branch-name>
   ```

If conflicts occur, Git will prompt you to resolve them manually before completing the merge.

---

## Deleting Branches
Once a branch has been merged and is no longer needed, it can be deleted:

```bash
git branch -d <branch-name>
```

To force delete (for unmerged branches):

```bash
git branch -D <branch-name>
```

---

## Summary
- **Branches** provide isolated environments for development.  
- **Creating branches** allows you to experiment without affecting the main code.  
- **Switching branches** lets you move between different work contexts.  
- **Merging branches** integrates changes back into another branch (commonly `main`).  
- **Deleting branches** keeps your repository clean once work is complete.  

Branches are essential for collaboration, parallel development, and maintaining clean project history.

---

## Learn More
- [Official Git Documentation: Branches](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)  
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials/using-branches)  
- [Git Merge Documentation](https://git-scm.com/docs/git-merge)  
