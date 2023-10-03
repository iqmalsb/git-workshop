# Git - Workshop

## Introduction
This repo serves as a guideline for introducing how git works for beginners. Feel free to use this however you want to. All credit goes to the original authors (see [References](#references) below). In this guide, there will be several terms used to convey meaning for an instruction or definition.

## Content
1. [Version Control & Git](#version-control--git)
2. [Preparation / Installation](#preparation--installation)
3. [Common Git Commands](#common-git-commands)
    - [git init](#git-init)
    - [git clone](#git-clone)
    - [git status](#git-status)
    - [git fetch / git pull](#git-fetch--git-clone)
    - [git add (git stage)](#git-add-git-stage)
    - [git commit](#git-commit)
    - [git push](#git-push)
    - [git branch](#git-branch)
    - [git checkout](#git-checkout)
4. [Advanced Git Commands](#advanced-git-commands)
    - [git merge](#git-merge)
    - [git rebase](#git-rebase)
    - [git stash](#git-stash)
5. [References](#references)

## Version Control & Git
Version control is a practice of software code management. One can view it as a perspective of accounting in finance. Every bit of transaction is somehow being recorded (i.e. amount and date). In software development, version control is the accounting practice. Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Preparation / Installation
To use git, you would have to install it on your local machine.

Go to [Git - Downloads page](https://git-scm.com/downloads) and follow the instructions provided according to your machine's OS and architecture (x64 or x86).

Verify your installation by opening your terminal and running the command `git --version` (or `git -v` for short).

## Common Git Commands
The following commands will be used primarily for your day-to-day use. There might be other commands that are not included in this README. You are encouraged to refer to the official [Git Documentation](https://git-scm.com/doc) for further information. You may also refer to their quick guides: [GitHub Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) | [Visual Git Cheat Sheet](https://ndpsoftware.com/git-cheatsheet.html)
### git init
This command creates an empty Git repository. This is usually the first required step for versioning your files.

Command:
`git init`

### git clone
Clones a repository into a new directory. 

Command:
`git clone [PATH]`
### git status
Show the working tree status. This command is typically paired with `git add` (executed after it) to see the changes in files before executing `git commit` ([See below](#git-commit))

Command:
`git status`
### git fetch / git pull
Download objects and refs from another repository

Command:
`git fetch`

Fetch from and integrate with another repository or a local branch

Command:
`git pull`

Difference between git fetch and git pull is primarily that git fetch only retrieves the information on what has been changed since (you can look at it like syncing device), whereas git pull retrieves the information and applies the changes on your local repo. 
### git add (git stage)
Add file contents to the index. The term 'stage' and its equivalent tenses usually refers to the same idea.

Command:
`git add [OPTIONS]`
### git commit
Record changes to the repository. This command will make the current branch that you are working on to have the latest 'entry'.

Command:
`git commit`
### git push
Update remote refs along with associated objects.

Command:
`git push [OPTIONS]`
### git branch
List, create, or delete branches. This is particularly useful if you are planning to make use of the Git branching strategies (Advanced topic, [see below](#references)).

Command:
`git branch [OPTIONS]`
### git checkout
Switch branches or restore working tree files. Depending on your workflow, you are required to not mix your tasks under a single branch especially if you are involved in multiple features or modules.

Command:
`git checkout [OPTIONS]`
## Advanced Git Commands
### git merge
Join two or more development histories together. This command is particularly common in applying the changes of a code from a branch (i.e. feature-branch) into another branch (i.e. production-branch).

Command:
`git merge [OPTIONS]`
### git rebase
Reapply commits on top of another base tip. This command makes your branch more streamlined (cleaner flow). However this is a very subjective opinion and should be used with the consensus of your team or organisation.

Command:
`git rebase [OPTIONS]`
### git stash
Stash the changes in a dirty working directory away. This command is very powerful and useful as to preserve changes without having to commit it (think of it like saving a draft before publishing).

Command:
`git stash [COMMNAD] [OPTIONS]`
## References
1. Official Git website | [https://git-scm.com/](https://git-scm.com/)
2. Git and GitHub for Beginners - Crash Course | [https://youtu.be/RGOj5yH7evk?si=dh6Mno4YeG6zzfQj](https://youtu.be/RGOj5yH7evk?si=dh6Mno4YeG6zzfQj)
3. Git Workflow - Atlassian Git Tutorial | [https://www.atlassian.com/git/tutorials/comparing-workflows](https://www.atlassian.com/git/tutorials/comparing-workflows)
