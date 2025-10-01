---
layout: default
title: Tags
nav_order: 8
---

# Tags
This page will cover tags in git, including what they are, how to use them and helpful commands to know when using tags in git.


### Table of Contents

1. [What are Tags in Git?](#What-are-Tags-in-Git?)  
2. [Creating Tags](#Creating-Tags)   
3. [Annotated Tags](#Annotated-Tags)  
4. [Once You've Created a Tag](#Once-You've-Created-a-Tag)  
5. [Additional Information Resources](#Additional-Information-Resources)  


## What are Tags in Git?

Tags in Git are like bookmarks for important events or milestones in your project.
They're often used to mark release points (v1.0.0, v1.1.0, etc.).

## Creating Tags
__Creating a new lightweight tag:__
```console
git tag <tag-name>
```

```console
git tag <tag-name> <commit hash>
```

This will tag the current or specified commit with the provided name.

__Tag Naming:__

Tag names should not include spaces. They should only include characters [a-z], [A-Z],
numbers [0-9] and the dash/hyphen [-].

## Annotated Tags
Additionally you can annotate your tags to provide additional metadata such as the tagger's name, email, date, and an optional message.



```console
git tag -a <tag-name> -m "your message here"
```

## Other Tag Commands
__Checkout to the tag:__ You can treat the tag like a branch/commit, and checkout to the tag's point in history. For example:

```console
git checkout <tag-name>
```

__List tags:__ You can list all the tags in the repository using git tag or git tag -l . To narrow the list based on a search pattern you can use:

```console 
git tag -l "<search-pattern>"
```

__Show tag information:__ If you have annotated tags, you can view the associated information with: 

```console
git show <tag-name> 
```

__Compare differences:__ You can compare the differences between the tagged state of the code and the current HEAD using:

 ```console
 git diff <tag-name>
 ```

__Deleting Tags:__ If you ever have the need to delete a tag, you can do so with:

```console
git tag -d <tagname>
```

__Sharing Tag:__ By default, using the git push command doesn’t transfer tags to remote servers. You will have to do it manually after creating them with: 

```console
git push origin <tagname>
```

## Additional Information Resources
- [Git Basics - Tagging](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
- [Atlassian - Git Tag](https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-tag)
- [Git - Tag](https://git-scm.com/docs/git-tag)

