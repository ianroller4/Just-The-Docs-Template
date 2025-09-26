---

title: Stashing Changes

nav\_order: 7

---

<!-- prettier-ignore-start -->
# Stashing Changes
{: .no_toc }

Git stash allows you to put aside changes that you don't want to commit immediately.

__Imagine a magic toy box:__

It Allows the kid to instantly clean their room, and when they want to play again, all toys are restored to their former positions.


### Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!--prettier-ignore-end-->

## When to use Stashing?
- When You want to switch branches, but you're in the middle of something and don't want to commit yet.
- You need to pull changes, but you have uncommitted work.

## Stashing in Action
To stash use the command: 

```
git stash
```


This command stashes your changes, leaving you with a clean working directory.

**Remember, it's only a temporary storage. Don't forget about your stashed changes!**

## Stash Stacks
Think of 'git stash' as creating a stack of saved changes.

You can stash multiple sets of
changes and Git will store them in a
LIFO (Last In, First Out) stack.

## Restoring Stashed Changes
To restore stashed changes, use the command: 

```
git stash pop
```

This Re-applies the changes and removes them from the stash.

If you want to keep use the changes but keep the stash, you can use the command:

```
git stash apply
```

This Re-applies the changes but keeps them within in the stash.

## Other Helpful Stash Commands

`git stash list` : Review all your stashes before deciding to apply or drop them.

`git stash drop ` : Removes the most recent stash from the stack without applying it.

`git stash branch <branchname> `: Creates a new branch based on the popped stash.

`git stash clear` : This command removes all your stashes.

`git stash pop 'stash@{n}` : Pop a specific stash seen in git stash list .

