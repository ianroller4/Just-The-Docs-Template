---
layout: default
title: Team Git Workflows
nav_order: 10
---
<!-- prettier-ignore-start -->
# Git Team Workflows
This page will cover working together in a team through git. This page will cover information about different workflows when working in a team, including brief overviews and how each workflow works.


### Table of Contents
{: .no_toc }

1. [Overview of Git Workflows](##Overview-of-Git-Workflows)  
2. [Centralized Workflow](##Centralized-Workflow)   
    - [How The Centralized Workflow Works](###How-The-Centralized-Workflow-Works)
3. [Feature Branch Workflow](##Feature-Branch-Workflow)  
    - [How The Feature Branch Workflow Works](###How-The-Feature-Branch-Workflow-Works)
4. [Forking Workflow](##Forking-Workflow)
    - [How The Forking Workflow Works](###How-The-Forking-Workflow-Works)
5. [Additional Information Resources](##Additional-Information-Resources)  

{:toc}

<!--prettier-ignore-end-->

## Overview of Git Workflows

With Git and GitHub, multiple developers can work on the same project without stepping on each other's toes. Teams working together can work in different ways to collaborate easier. 

Git workflows are methods or procedures that dictate how developers interact with the Git system to achieve effective team collaboration.

There are several popular workflows used by teams:

- __Centralized Workflow__
- __Feature Branch Workflow__
- __Forking Workflow__

## Centralized Workflow
All developers work directly on a single branch, often main or master. This workflow is quite Simple and similar to Subversion-style workflows. However it is not as powerful or flexible as the other workflows. When working within this workflow merging can be problematic as everyone is working within the same branch.

This workflow is suitable for small teams and projects but gets more difficult as the team and project scales bigger. 


### How The Centralized Workflow Works
1. __Initialization:__ One team member creates the repository with an online remote.
2. __Cloning:__ Each team member creates a local copy by "cloning" the remote.
3. __Working Locally:__ Developers work on the project, committing to their local repo.
4. __Resolving Conflicts:__ When a developer is ready to share their changes, they must pull outstanding changes from the remote, and resolve merge conflicts as required.
5. __Pushing to Remote:__ The developer can now push their changes to the central
repo.
6. __Synchronizing Team:__ Others can now pull from the central repo to locally
incorporate the latest changes.

## Feature Branch Workflow

This workflow works similar to the centralized workflow, however it differs in how all feature development or bug fixes are done in different dedicated branches. New development is isolated from the main branch rather than all members working in main branch. 

Some advantages of working in this workflow are:

- It makes it easy to discard experimental changes due to them being on their own individual branch.

- Code review are much easier due to the creation of pull requests.

*Note: This workflow is sometimes called Github Flow.*


### How The Feature Branch Workflow Works
This workflow works similar the Centralized Workflow, however it differs through:

- __Branching:__  New features or fixes are developed locally in a new short-lived branch.

- __Resolving Conflicts:__ Remote commits by other developers can be pulled into the local feature branch, with merge conflicts resolved as required.

- __Pushing to Remote:__ Completed and resolved branches are then pushed to the remote repo.

- __Requesting a Remote Merge:__ A pull request is next initiated on the git hosting service (example: GitHub).

- __Reviewing:__ One or more team members review the pull request before merging it into the main remote branch.

Note: Pull requests can be sent back unmerged if rework is deemed necessary.

## Forking Workflow
This workflow is most often used for open source projects, in this workflow each developer gets not only their own local repository, but also a server-side copy of the project through forking.

*Forking is the process of creating a personal copy of another user's repository.*

Within this workflow developers push to their own server-side repositories rather than one main one. Changes are shared to the main project via pull requests from their personal public repository.

The maintainer of the main project has the final say on what is merged into the official repository.


### How The Forking Workflow Works
This workflow works similar to the Feature Branch workflow, however it differs through:

- __Forking:__ Instead of creating branches, each team member creates a fork of the project on the git hosting service.

- __Cloning:__ Team members clone their remote fork to a local repo.

- __Adding an Upstream:__ Team members configure a secondary remote called upstream that points to the official repo.

- __Resolving Conflicts:__ Remote commits from upstream can be pulled into the local feature branch, with merge conflicts resolved as required.

- __Pushing to Remote:__ Local feature branches are pushed to the forked remote.

- __Requesting a Remote Merge:__ Pull request are initiated to request merges from the remote fork to the official upstream repo.

## Additional Information Resources
- [Atlassian - Centralized Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows#centralized-workflow)
- [Atlassian - Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)
- [Atlassian - Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)

