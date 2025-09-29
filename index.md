---
title: Home
layout: home
nav_order: 1
---

# Home

Welcome to our Git Wiki. This website serves as a resource for game developer programmers and artists to quickly look up and find the information they need regarding Git and GitHub. There is the homepage. Here you will find information about version control in software development, what git is, links to resources to learn more about Git in detail, and finally brief biographies about the contributors to this site.

## Table of Contents
1. [The Role of Version Control in Software Development](#the-role-of-verison-control-in-software-development)
    - [Version History: The Backbone of Change Tracking](#1-version-history-the-backbone-of-change-tracking)  
    - [Collaborating Without Colliding](#2-collaborating-without-colliding)  
    - [Fix Mistakes with Confidence](#3-fix-mistakes-with-confidence)  
    - [Isolated Development with Branches](#4-isolated-development-with-branches)  
    - [Built-In Accountability and Transparency](#5-built-in-accountability-and-transparency)  
    - [Powering Automation: CI/CD Integration](#6-powering-automation-cicd-integration)  
    - [Code Reviews Made Easy](#7-code-reviews-made-easy)  
    - [Tools That Make It Possible](#8-tools-that-make-it-possible)  
    - [The Real-World Impact of Using Version Control](#9-the-real-world-impact-of-using-version-control)  
2. [What is Git](#what-is-git)
    - [Pros of Git](#pros-of-git)
    - [Cons of Git](#cons-of-git)
3. [Learn More (General Information)](#10-learn-more-general-information)
4. [Contributor Biographies](#contributor-biographies)
    - [Hilandrei Caligagan](#hilandrei-caligagan)
    - [Morgan Klassen](#morgan-klassen)
    - [Ian Roller](#ian-roller)


## The Role of Verison Control in Software Development
Version control is a critical tool in software development, enabling teams and individuals   
to manage changes to code, collaborate effectively, and maintain a reliable history of project evolution.   
It ensures that development processes are organized, traceable, and resilient to errors.

### 1. Version History: The Backbone of Change Tracking

Version control systems maintain a detailed history of every change made to the codebase. Each change is saved as a **commit**, which includes:

- What was changed
- Who made the change
- When it was made
- A message describing the reason for the change

This allows developers to:

- View a timeline of code evolution
- Compare different versions of files
- Identify when a bug was introduced
- Understand the intent behind changes

In tools like Git, this history is stored locally and remotely, making it easy to backtrack or audit the project at any point.

### 2. Collaborating Without Colliding

Modern development is highly collaborative. Version control allows multiple developers to work on the same codebase at the same time **without interfering** with one another.

Key features include:

- **Branches**: Independent copies of the code where developers can work on features or bug fixes.
- **Merges**: Safely integrate changes from multiple branches into a shared branch.
- **Conflict resolution**: Handles overlapping edits and flags issues that need manual intervention.

This structure allows for **parallel development**, which accelerates delivery and reduces bottlenecks.

### 3. Fix Mistakes with Confidence

Mistakes are inevitable — but version control ensures they aren't permanent.

With tools like Git, developers can:

- **Revert** specific commits
- **Reset** to a previous project state
- Use **tags** to mark stable versions like releases

This allows teams to recover quickly from bugs, failed experiments, or even accidental deletions, providing a strong safety net throughout the development process.

### 4. Isolated Development with Branches

Branching is a powerful feature that enables developers to isolate changes before integrating them into the main project.

Common use cases:

- New features (`feature/payment-integration`)
- Hotfixes (`hotfix/login-bug`)
- Experiments or refactors

After work is complete, the branch is tested, reviewed, and then merged back into the main branch (e.g., `main` or `dev`). This keeps the production codebase clean and stable, while allowing fast-paced innovation in parallel.

### 5. Built-In Accountability and Transparency

Every commit is tied to a specific user, with a timestamp and message. This offers:

- Clear visibility into **who made which change**
- A documented rationale for each decision
- Easy collaboration across teams and time zones

For managers or auditors, version control provides a **transparent, auditable trail** of how a product evolves — especially important in industries with compliance requirements.

### 6. Powering Automation: CI/CD Integration

Version control is the core trigger for **Continuous Integration and Continuous Deployment (CI/CD)** workflows.

When a developer pushes changes to the repository, automated tools can:

- Run unit tests
- Build the application
- Deploy to staging or production environments

Popular tools that integrate directly with Git include:

- [GitHub Actions](https://github.com/features/actions)
- [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)
- [Jenkins](https://www.jenkins.io/)

This automation speeds up release cycles and improves reliability.

### 7. Code Reviews Made Easy

Version control simplifies the code review process. Platforms like GitHub, GitLab, and Bitbucket offer:

- **Pull requests** or **merge requests** for proposing changes
- Inline commenting on specific lines of code
- Approvals and requested changes before merging

Code reviews help improve quality, share knowledge, and enforce team standards — and version control makes the process smooth and structured.

### 8. Tools That Make It Possible

Here are some popular version control systems:

- [**Git**](https://git-scm.com/) – Distributed, open-source, widely adopted
- [**Subversion (SVN)**](https://subversion.apache.org/) – Centralized, often used in legacy projects
- [**Mercurial**](https://www.mercurial-scm.org/) – Lightweight and simple
- [**Perforce (Helix Core)**](https://www.perforce.com/products/helix-core) – Used in enterprise and gaming

Git is by far the most popular today, but each has its place depending on project needs.

### 9. The Real-World Impact of Using Version Control

**Without Version Control:**

- Developers accidentally overwrite each other’s work
- It’s hard to track down bugs or understand changes
- Releasing stable versions is risky and manual
- Team collaboration is error-prone

**With Version Control:**

- Every change is documented and reversible
- Teams collaborate asynchronously with confidence
- Releases are safer, faster, and more frequent
- Development is more organized, auditable, and scalable

Version control transforms software development from risky trial-and-error into a **disciplined, manageable process**.

## What is Git

Git is a free and open source distributed version control system. Git keeps track of the changes we make to our files as we make them. When combined with an online version control site such as GitHub (where this website is hosted) Git can be used to collaborate with others remotely.

### Pros of Git

Here are a few reasons for you to use Git:

1. You can commit as many or as little times as you like.
2. If a mistake is committed or you just want to go back to a previous version it is possible to go back to previous commits.
3. Allows users to work with others without having a consistant internet connection.

### Cons of Git

Here are a few reasons for you not to use Git:
1. Git is not that user friendly for non technical individuals.
2. There is no built in support for large repos.
3. There is no built in support for locking binary assets.

## Learn More

- [Pro Git Book (Free)](https://git-scm.com/book/en/v2)
- [What Is Version Control?](https://www.spiceworks.com/tech/devops/articles/what-is-version-control)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- [GitLab – Version Control with Git](https://docs.gitlab.com/ee/topics/git/)
- [Codecademy – Learn Git](https://www.codecademy.com/learn/learn-git)
- [CI/CD Explained – GitHub](https://docs.github.com/en/actions/learn-github-actions/introduction-to-github-actions#understanding-github-actions)
- [Git Branching Strategies – Atlassian](https://www.atlassian.com/git/tutorials/comparing-workflows)


## Contributor Biographies

### Hilandrei Caligagan 

### Morgan Klassen

### Ian Roller
Current student at RRC Polytech in the Game Development Programming program. Graduated from the University of Manitoba with a degree in Computer Engineering in 2023. Currently learning to write and draw. Likes basketball, reading, and video games.


[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: [https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md](https://github.com/StungEye-RRC/Just-The-Docs-Template#readme)
[Jekyll]: https://jekyllrb.com
[Markdown Syntax]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
