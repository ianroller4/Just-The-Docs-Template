---
layout: default
title: Undoing in Git
nav_order: 4
---

# Undoing in Git

There are four main ways of undoing changes in Git. These are, `checkout`, `reset`, `revert`, and `clean`. This page will describe each method, how to use it, and when to use it.

## Checkout

`checkout` is the simplist type of private undoing in Git. Using `checkout` will discard any uncommited changes you have made locally on your computer.

### How to Use

To use `checkout`, in the command terminal in the working folder `checkout` enter:

```console
~$ git checkout <path-or-filename>
```

For example, say you wanted to undo chanages you have made locally to the `README.md` file, you would do:

```console
~$ git checkout README.md
```

Or to revert all files to the most recent commit:

```console
~$ git checkout .
```

### When to Use
`checkout` should be used in the following two cases:

1. The changes you wish to undo have not yet been committed
2. You wish to revert to the most recently committed version of a file or files 

> **Warning:**
> `checkout` is slightly dangerous as the discarded changes cannot be recovered.

## Reset

`reset` can be used to undo one or more commits in our **local** repository.

`reset` has two different ways to undo.

1. Hard Reset - Changes your working directory to match a specific commit
2. Soft Reset - Keeps your changs in the working directory, but still resets the HEAD

> **Note:** The result of `soft reset` is a little weird.

### How to Use

To use `hard reset`, in the command terminal in the working folder enter:

```console
~$ git reset --hard [commit id]
```
> **Warning:**
> Uncommitted changes are lost and all files are reset to the specified commit.

To use `soft reset`, in the command terminal in the working folder enter:

```console
~$ git reset --soft [commit id]
```
> **Weird:**
> HEAD and working directory may differ if you had uncommited changes.

### When to Use

`reset` should be used when you wish to undo one or more commits in your **local** repository.

## Revert

`revert` creates a new commit that undoes a changes from a specific commit.

`revert` is typically used to undo a commit that has been shared with others.

`revert` is the safest choice when undoing as reverting maintains commit history.

### How to Use

To use `revert`, in the command terminal in the working folder enter:
```console
~$ git revert <commit id>
```

### When to Use

`revert` should be used when you wish to run a specific commit in reverse.

## Clean

Where other undoing commands in Git deal with files that are tracked with version control, `clean` deals with files that are not tracked.

### How to Use

To use `clean`, in the command terminal in the working folder enter:
```console
~$ git clean 
```
### When to Use

`clean` should be used when there are temporary files and / or folders that need to be removed before committing.