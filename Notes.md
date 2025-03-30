# Git & Github

Git is a version control system that is used to track changes to your files.
Version control systems are used to manage the history of your code. They allow us to track changes to our files and to collaborate with others

Where as Github is a web-based hosting service for Git repositories. Github is an online platform that allows us to store and share your code with others.
Alternative Timeline is called branch.

## Checking Git Version

    git --version

## Repository

Folder is called repositories.It is a collection of files and directories that are stored together. It is a way to store and manage our code.

## Checking status:-

    git status

## Setting up for the first time globally

    git config --global user.email "your-email@example.com"
    git config --global user.name "Your Name"

## To check what changes are made in config files

    git config --list

## Creating a repo:-

    git status
    git init

## Flow:-

    Write -> Add -> Staging Area -> Commit -> Repository -> Push -> Github

## Stage:-

Stage is a way to tell git to track a particular file or folder. You can use the following command to stage a file

    git add <file> <file2> 
                            or
    git add .

## Commit:-

commit is a way to save your changes to your repository. It is a way to record your changes and make them permanent.When you commit your changes, you are telling git to save them in a permanent way

    git commit -m "your message"

## Logs

    git log
                            or
    git log --oneline

This command will show you the history of your repository. It will show you all the commits that were made to the repository. You can use the --oneline flag to show only the commit message. This will make the output more compact and easier to read.

## gitignore and gitkeep

gitignore is a file that makes sure important files like env are not tracked.
Its usually kept at the root of project and all the files and folders that we want to ignore are listed in it.
Where as gitkeep is the exact opposite it tells git to track empty folders and it is usually kept in the empty folder that we want to track.

## Branches

Branch is a way to create a copy of your code. It is a way to work on a new feature or a new bug fix without affecting the main code.

We can check our branch by using the following command

    git branch

We can create a branch using the following command

    git branch <branch-name>

we can move to a branch using the following command

    git switch <branch-name>

We can use a -c flag to create a new branch and switch to it at the same time

    git switch -c <branch-name>

we can use checkout to switch to a branch

    git checkout <branch-name>

Difference between switch and checkout is that switch is a new command that is used to switch between branches. It is a more user-friendly way to switch between branches. Checkout is an older command that is used to switch between branches. It is a more powerful command that can be used to do more things, but it is also more complex and harder to use.

We can delete a branch using the following command

    git branch -d <branch-name>

## Head

Head is a pointer that points to the current branch. It is a way to keep track of where you are in your repository. You can use the following command to check where your head is pointing

    git show-branch
                            or
    git show-branch --all

## Merging

Merging is a way to combine two branches together. It is a way to take the changes from one branch and apply them to another branch. You can use the following command to merge two branches together

    git merge <branch-name>

## Branches

Branches are used to work on different features or bug fixes at the same time. They allow you to work on multiple things at once without affecting the main code. You can create a branch for each feature or bug fix that you are working on. Once you are done with the feature or bug fix, you can merge it back into the main branch.
You can use the following command to create a branch

    git branch <branch-name>

## Conflicts

Conflicts occur when two branches have changes that are incompatible with each other. This can happen when two people are working on the same file at the same time. When this happens, git will not be able to merge the two branches together. You will need to resolve the conflicts manually. You can use the following command to see what files have conflicts

    git status
    git diff --name-only --diff-filter=U

We can find the difference between both branches and decide which code to keep
