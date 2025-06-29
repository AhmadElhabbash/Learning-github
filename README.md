# Git and Github

## Introduction

### Version Control system (vcs) like Git

Aversion Control System is like atime machine for your code .It allows
you to:
-Track Changes
-Go back in time
-Collaborat easily

### Everyday Analogy

Imagine you are writing a big essay in Microsoft Word.

- You make a lot of edits over time, but you forgot what you changed.
- if you accidentally delete a section, there is no way to get it back unless you saved a new file.
- if you and a friend edit the same file or section, you will end up duplicate versions like essay-final-v2.0.0.docx.
  A version control system fixes these problems by:

- Keeping a history of all changes.
- Allowing you to undo mistakes by restoring old versions.
- Merging edits from multiple people into a single file without conflicts.

### Why developers use Git and Github

In coding projects:

- A team might work on the same codebase, without a VCS, changes could overwrite each other.
- Bugs might be appear after changes, and a VCS helps pinpoint the issue by reviewing past changes.
- VCS tools like Git automate this process, making it fast and reliable.

### Getting Started with Git

- Installing Git

### Configuring Git

Setting up Git for the first time:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com" # please use your GitHub email, if you do not have one, use the same Git email when you create a GitHub account
```

To check your Git configuration:

```bash
git config --list
```

### Basic Git Terminology:

### Repository (Repo) Is a container for your project and its entire history.

- Think of it as a folder that tracks all your code, and their changes.

There are two types of repositories:

- **Local repository**: Stored on your computer.
- **Remote repository**: Stored on a platform, like GitHub.

  ### Creating your first (local) repository:

```bash
mkdir git-github-crash-course
```

```bash
cd git-github-crash-course
```

```bash
git init //mean start git repo

```

### Commits

A commit is a snapshot of your code at a specific point in time.

It saves your changes so you can review or go back to them later.

Think of it as taking a photo of your project after making edits.

### git status

## What it does?

- Shows the current state of your working directory and staging area.
- Tells you which files have been modified, added, or deleted.
- Helps you track what changes are ready to commit and what needs to be staged.

```bash
git status
```

### git add file-name

### What it does?

- Moves changes from the working directory to the staging area, preparing them for a commit.
- Files must be staged before they can be committed.

```bash
git add file-name
```

```bash
git add file-name other-file-name
```

```bash
git add -A
```

```bash
git restore --staged file-name
```

### What it does?

- Removes files from the staging area, but keeps the changes in the working directory.
- It "un-stages" files without discarding edits.

### commit

### What it does?

- Takes a snapshot of the files in the staging area and saves it in the repository's history.

````bash
git commit -m "Commit Message"```
````
