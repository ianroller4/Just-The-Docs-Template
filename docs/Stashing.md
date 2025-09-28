---
layout: default
title: Stashing Changes
nav_order: 7
---

<!-- prettier-ignore-start -->
# Stashing Changes
{: .no_toc }

Stashing changes in git allows you to put aside changes that you don't want to commit immediately.

An analogy would be a kid's magic toy box:

It allows the kid to instantly clean their room, and when they want to play again, all toys are restored to their former positions.


### Table of Contents
{: .no_toc }

1. [When to use Stashing?](##When-to-use-Stashing?)  
2. [Stashing in action](##Stashing-in-action)   
3. [Restoring Stashed Changes](##Restoring-Stashed-Changes)  
4. [Other Helpful Stash Commands](##Other-Helpful-Stash-Commands)  
5. [Additional Information Resources](##Additional-Information-Resources)  

{:toc}

<!--prettier-ignore-end-->

## When to use Stashing?
Stashing is useful for whenever you need to put away your work temporarily.

For Example:
- When you want to switch branches, but you're in the middle of something and don't want to commit yet.
- You need to pull changes, but you have uncommitted work.

## Stashing in Action
To stash use the command: 

```console
git stash
```

This command stashes your changes, leaving you with a clean working directory.

You can also use `git stash push` for additional functionality like specifying a path/file with pathspec.

**Remember, it's only a temporary storage. Don't forget about your stashed changes!**

## Restoring Stashed Changes
To restore stashed changes, use the command: 

```console
git stash pop
```

This re-applies the latest changes and removes them from the stash.

*Git stores stashed changed them in a LIFO (Last In, First Out) stack, so pop will restore the latest stashed change.*

If you want to apply the stashed changes but keep them within the stash aswell, you can use the command:

```console
git stash apply
```

This re-applies the changes but keeps them within in the stash. 

This can be helpful if you want to apply stashed changes to multiple different branches.

## Other Helpful Stash Commands

`git stash list` : Review all your stashes before deciding to apply or drop them.

`git stash drop ` : Removes the most recent stash from the stack without applying it.

`git stash branch <branchname> `: Creates a new branch based on the popped stash.

`git stash clear` : This command removes all your stashes.

`git stash pop 'stash@{n}` : Pop a specific stash seen in git stash list .

## Additional Information Resources

- [Git - Stashing](https://git-scm.com/docs/git-stash)
- [Atlassian - Git Stash](https://www.atlassian.com/git/tutorials/saving-changes/git-stash#partial-stashes)