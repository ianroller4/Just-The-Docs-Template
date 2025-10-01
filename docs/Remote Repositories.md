# Remote Repositories in Git

Remote repositories in Git are versions of your project that are hosted
on the internet or network. They enable collaboration, backup, and
sharing by allowing multiple people to work on the same project.
Developers can fetch, pull, and push changes to keep local and remote
copies in sync.

------------------------------------------------------------------------

## Table of Contents

- [What Are Remote Repositories?](#what-are-remote-repositories)
- [Cloning a Remote Repository](#cloning-a-remote-repository)
- [Viewing Remotes](#viewing-remotes)
- [Adding a Remote](#adding-a-remote)
- [Removing a Remote](#removing-a-remote)
- [Fetching Changes](#fetching-changes)
- [Pulling Changes](#pulling-changes)
- [Pushing Changes](#pushing-changes)
- [Summary](#summary)
- [Learn More](#learn-more)

------------------------------------------------------------------------

## What Are Remote Repositories?

A **remote repository** is a copy of your project that lives on a remote
server. Unlike your local repository, which only you can access, remote
repositories are typically shared via platforms like GitHub, GitLab, or
Bitbucket. They allow teams to collaborate by synchronizing code.

------------------------------------------------------------------------

## Cloning a Remote Repository

To create a local copy of a remote repository, use:

    git clone <repository_url>

This copies the entire project history and sets up a default remote
called **origin**.

------------------------------------------------------------------------

## Viewing Remotes

You can check which remotes are linked to your repository with:

    git remote -v

This lists remote names and their corresponding **fetch** and **push** URLs.

------------------------------------------------------------------------

## Adding a Remote

To add a new remote repository, use:

    git remote add <name> <url>

For example:

    git remote add origin https://github.com/user/project.git

This links a remote repository to your local repository.

------------------------------------------------------------------------

## Removing a Remote

To remove a remote reference:

    git remote remove <name>

This removes the connection between the remote and local repository.

It does not delete any actual repository, just the connection.

------------------------------------------------------------------------

## Fetching Changes

Fetching updates your local repository with new changes from a remote
without merging them:

    git fetch <remote_name>

This downloads new commits, branches, and tags from the remote repository, and updates your local record of the remote.

------------------------------------------------------------------------

## Pulling Changes

Pulling both fetches and merges remote changes into your current branch:

    git pull <remote_name> <branch_name>

This updates your branch with commits from the remote and merges them.

You may need to resolve merge conflicts if others have worked on the same files as you.

------------------------------------------------------------------------

## Pushing Changes

Pushing sends your local commits to the remote repository:

    git push <remote_name> <branch_name>

This sends your commits to the specified branch on the remote so collaborators can access them.

You will have to make a pull request in order to merge your branch with main on the remote.

------------------------------------------------------------------------

## Summary

- Remote repositories provide a shared location for collaboration.
- Clone projects from a server with `git clone`.
- Connect local repositories to remotes with `git remote add`.
- Disconnect local repositories from remotes with `git remote`.
- Show current remote connections with `git remote -v`
- Fetch and pull updates from remotes with `git fetch` and `git pull`.
- Push new commits to the remote with `git push`.

------------------------------------------------------------------------

## Learn More

-   [Official Git Documentation on Remote Repositories](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)
-   [GitHub Guides: Hello World](https://guides.github.com/activities/hello-world/)
-   [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials/setting-up-a-repository)
