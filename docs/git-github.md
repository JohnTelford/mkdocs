## Version Control

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later

## VCS
A version control system, or VCS, tracks the history of changes as people and teams collaborate on projects together. As developers make changes to the project, any earlier version of the project can be recovered at any time.

---

## About version control and Git

[About version control and Git](https://docs.github.com/en/get-started/using-git/about-git#about-version-control-and-git)

## GitHub

GitHub is a Distributed Version Control Systems enabling multiple teams to work separately on the same project without having an impact on the work of others. GitHub manages an online web hosted Central Website Repository containing all project files. It is a unified source of truth. It helps teams collaborate and maintain the entire history of project file changes, and helps answer the questions who changed what, where, when, and why for the lifetime of the project

## Getting Started

[Getting Started](https://docs.github.com/en/get-started/using-git/about-git#about-version-control-and-git)

## How GitHub works

[How GitHub works](https://docs.github.com/en/get-started/using-git/about-git#how-github-works)

---

## Basic Git Commands

[Basic Git Commands](https://docs.github.com/en/get-started/using-git/about-git#basic-git-commands)

To use Git, developers use specific commands to copy, create, change, and combine code. These commands can be executed directly from the command line or by using an application like GitHub Desktop. Here are some common commands for using Git:

### git init

`git init` initializes a brand new Git repository and begins tracking an existing directory. It adds a hidden subfolder within the existing directory that houses the internal data structure required for version control.

### git clone

`git clone` creates a local copy of a project that already exists remotely. The clone includes all the project's files, history, and branches.

### git add

`git add` stages a change. Git tracks changes to a developer's codebase, but it's necessary to stage and take a snapshot of the changes to include them in the project's history. This command performs staging, the first part of that two-step process. Any changes that are staged will become a part of the next snapshot and a part of the project's history. Staging and committing separately gives developers complete control over the history of their project without changing how they code and work.

### git commit

`git commit` saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that's been staged with git add will become a part of the snapshot with git commit.

### git status

`git status` shows the status of changes as untracked, modified, or staged.

### git branch

`git branch` shows the branches being worked on locally.

### git merge

`git merge` merges lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the main branch for deployment.

### git pull

`git pull` updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment.

### git push

`git push` updates the remote repository with any commits made locally to a branch.

### Full Reference Guide To Git Commands

[Full Reference Guide To Git Commands](https://git-scm.com/docs).

---

## Models for collaborative development

[Models for collaborative development](https://docs.github.com/en/get-started/using-git/about-git#models-for-collaborative-development)

## Importing a Git repository using the command line

[Importing a Git repository using the command line](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/importing-a-git-repository-using-the-command-line)

