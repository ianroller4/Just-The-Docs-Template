---
layout: default
title: Resolving Merge Conflicts
nav_order: 6
---

# Merge Conflicts
This page will go over all someone would need to know about merge conflicts including what they are, when they occur, and how to resolve merge conflicts.

## Table of Contents
1. [What is a Merge Conflict](#what-is-a-merge-conflict)
2. [When Merge Conflicts Occur](#when-merge-conflicts-occur)
3. [Resolving Merge Conflicts](#resolving-merge-conflicts)
4. [Additional Resources](#additional-resources)

## What is a Merge Conflict
A merge conflict is when two git branches cannot be cleanly merged together because different work was done on the same part in both branches, thus Git does not know which change should be kept. Instead of Git trying to fix it itself, it results in a merge conflict.

## When Merge Conflicts Occur
As mentioned merge conflicts occur when work done in two separate branches is done on the same part. When this happens Git will notify you and mark the areas that are in conflict in your files.

To clearly show what is in conflict Git uses special markers to indicate the start and end of conflicted area. These markers are as shown:

`<<<<<<< HEAD` - Shows the start of the changes in the current branch

`=======` - Separator between the changes from each branch

`>>>>>>> branch-name` - Shows the end of the changes in the other branch

## Resolving Merge Conflicts
To resolve a merge conflict follow this three step process:
1. Edit the file to fix the conflicting changes.
    - *Be sure to remove the conflict markers*
2. Add the file(s) to the staging area with `git add`
3. Commit the file(s) that has been fixed with `git commit`

## Additional Resources
1. [GitHub Docs - About Merge Conflicts](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)
2. [GitHub Docs - Resolving Merge Conflicts](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line)
3. [Atlassian - Merge Conflicts](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts)