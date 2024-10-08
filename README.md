# Git Basics

## Git commands - Handy Sheet 
<br>
### Cloning the existing online repository

```bash
# FORK
# First Fork the repository you want to clone.
# This will create a copy on your GitHub that you will be allowed to change
# CLONE
# Copy the url of your repository copy and run the command
git clone <repository url>

# OPEN THE PROJECT
cd <project folder name>
code .

```

<br>
# Creating commits

```bash
# git add <filename>
git add .
git status
git commit -m 'Initial commit'
git status
git push origin <branchname>
```
<br>

# Initializing git in a new project

```bash
# Initialize git repository in the current project
# While in the root directory of your project
git init
# List all the files in the directory, this will show you .git directory
ls -a
# Create a connection between local and online repository
git remote add origin <github repo url>
# Check the list of repositories connected to local
# This will show the repo that we just connected to
git remote -v
# Check the status of the files in the project and the staging area.
git status
# Add all unstaged (red) files to the stagging area (prepare to commit)
# git add <filename>
git add .
# Check the status of the files and the staging area (stagged files are now green).
git status
# Create a commit (snapshot)
git commit -m 'Initial commit'
# Stagging area is now clear
git status
# Push code to the GitHub repository
git push origin <branch name>
# Check the history of all existing commits
git log
# Notice that each commit has a hash identifier
# Hash identifiers are used to move through to the history (by repointing the HEAD)
```
<br>

### Connecting the local repository to the online (GitHub) repository

```bash
# First create the GitHub repository on the github.com
#  ...
#  ...

# Create a connection between local and online repository
git remote add origin <github repo url>

# Check the list of repositories connected to local
# This will show the repo that we just connected to
git remote -v

```
