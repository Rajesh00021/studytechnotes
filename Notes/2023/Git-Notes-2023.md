# What is Git?

Git is a version control system that allows you to manage and track changes to your code over time. It is a popular tool among software developers for collaboration and maintaining code quality.

At its core, Git allows you to create a "repository" that contains all of the code and files for your project. You can then make changes to these files, and Git will track these changes over time. You can also create different "branches" of your codebase to experiment with new features or fixes without affecting the main codebase.


### Let's learn basic git commands

In this section, you will learn the essential Git commands. These basic Git commands are the foundation to learn more advanced commands. Here are the nine useful Git commands.

### 1 git config

The Git config command is super helpful. Especially when you are using Git for the first time, or you have a new Git installation. This command will set up your identity - Name and Email address. And this information will be used with every commit.

**Usage**

`$ git config --global user.name "Your name"`

`$ git config --global user.email "Your email"`

### 2 git version

As its name implies, it's just to check which version of Git you are using. At the moment, writing this guide, the latest version of Git for Windows is 2.31.1. It was released on 19th December 2022.

**Usage**

`$ git version`

### 3 git init

This is probably the first command you use to start a new project in Git. This command will create a blank new repository, and then you can store your source code inside this repo.

**Usage**

`$ git init`

Or you can use the repository name with your git init command.

`$ git init <your repository name>`

4\. git clone

The git clone command will use an existing repository to copy. There is one main difference between the git init and git clone.

You will use the Git clone when you need to make a copy on an existing repository. The git clone command internally uses the git init command first and then checks out all its contents.

**Usage**

`git clone <your project URL>`

### 5 git add

The Git add command will add all the new code files or modified files into your repository. This command offers different options to add files and folders.

Here is the usage of the Git add command.

**Usage**

`$ git add your_file_name` (it will add a single file to your staging area)

`$ git add *` ( this option will add all the modified and new files to the staging area)

### 6 git commit

This Git command is essential. Your project quality may drop if you will not use this command appropriately. There is another article about how to use Git commands property, and you can read that [here](https://acompiler.com/git-best-practices/).

In simple words, the Git commit will add your changes to your local repository.

**Usage**

`$ git commit -m “your useful commit message”`

### 7 git status

This Git command is convenient to see how many files are there which need your attention. You can run this command at any time.

You can use it in between Git add, and Git commits to see the status.

**Usage**

`$ git status`

### 8 git branch

Most of the time, you have multiple branches in your Git repository. In simple terms, the branch is an independent line of code development.

With the Git branch command, you can manage your branches effectively. There are many different options and switches in the Git branch.

**Usage**

(i) To list all branches:

`$ git branch`

(ii) To create a new branch:

`$ git branch <branch_name>`

(iii) To delete a branch:

`$ git branch -d <branch_name>`

9\. git checkout

This Git command is used to switch between branches. In simple words, here is the syntax to switch to another branch.

**Usage**

`$ git checkout <branch_name>`

The following command is widely used to create a new branch and switch in, we can say this shortcut.

`$ git checkout -b <your_new_branch_name>`

## Let's learn intermediate level git commands

These Git commands are super helpful if you need to collaborate with your team, and share your code with others.

### 10 git remote

Git remote command acts like a border, and If you need to connect with the outside world, you have to use the Git remote command. This command will connect your local repository to the remote.

**Usage**

`$ git remote add <shortname> <url>`

Example

`$ git remote add origin https://dev.azure.com/aCompiler/_git/DemoProject`

### 11 git push

Once you are connected with the remote repository (with the help of the git remote command), it's time to push your changes to that repository.

**Usage**

`$ git push -u <short_name> <your_branch_name>`

**Example**

`$ git push -u origin feature_branch`

You should have the origin and upstream setup before you use Git to push. And here is the command to set up upstream.

**Usage**

`$ git push --set-upstream <short_name> <branch_name>`

**Example**

`$ git push --set-upstream origin feature_branch`

### 13 git fetch

When you need to download other team members' changes, you have to use git fetch.

This command will download all information for commits, refs, etc., so you can review it before applying those changes in your local repository.

**Usage**

`$ git fetch`

### 14 git pull

The Git pull command downloads the content (and not the metadata) and immediately updates your local repository with the latest content.

**Usage**

`$ git pull <remote_url>`

### **15\. git stash**

This Git command temporarily stores your modified files. You can work in stashed with the following Git command.

**Usage**

`$ git stash`

And you can view all of your stashes with the following command

`$ git stash list`

And if you need a apply a stash to a branch, simply use apply

`$ git stash apply`

### 16 git log

Git log, you can see all the previous commits with the most recent commit appearing first.

**Usage**

`$ git log`

it will show you all the commits of the currently checked-out branch, but you can force it to see all the commits of all the branches with all options.

`$ git log --all`

### A resource to Learn All Commands

[Check](https://www.youtube.com/watch?v=apGV9Kg7ics)
