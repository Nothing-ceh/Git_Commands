# Git_Commands

 Here is a comprehensive list of Git commands along with examples for each.

Configuration
Configure user information for all local repositories

sh
Copy code
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
Check configuration settings

sh
Copy code
git config --list
Repository Management
Initialize a new Git repository

sh
Copy code
git init
Clone an existing repository

sh
Copy code
git clone https://github.com/user/repository.git
Basic Snapshotting
Add files to the staging area

sh
Copy code
git add filename
git add .
Commit changes

sh
Copy code
git commit -m "Commit message"
View the commit history

sh
Copy code
git log
Branching and Merging
Create a new branch

sh
Copy code
git branch new-branch
List branches

sh
Copy code
git branch
Switch to a branch

sh
Copy code
git checkout branch-name
Create and switch to a new branch

sh
Copy code
git checkout -b new-branch
Merge a branch into the current branch

sh
Copy code
git merge branch-name
Delete a branch

sh
Copy code
git branch -d branch-name
Remote Repositories
Add a remote repository

sh
Copy code
git remote add origin https://github.com/user/repository.git
View remote repositories

sh
Copy code
git remote -v
Fetch changes from the remote repository

sh
Copy code
git fetch
Push changes to the remote repository

sh
Copy code
git push origin branch-name
Pull changes from the remote repository

sh
Copy code
git pull origin branch-name
Undoing Changes
Unstage a file

sh
Copy code
git reset HEAD filename
Revert changes in a file

sh
Copy code
git checkout -- filename
Amend the last commit

sh
Copy code
git commit --amend -m "New commit message"
Revert a commit by creating a new commit

sh
Copy code
git revert commit-id
Viewing Changes
Show changes in the working directory

sh
Copy code
git status
Show changes between the working directory and the index

sh
Copy code
git diff
Show changes between the index and the last commit

sh
Copy code
git diff --cached
Show changes between two commits

sh
Copy code
git diff commit1 commit2
Stashing and Cleaning
Stash changes

sh
Copy code
git stash
List stashed changes

sh
Copy code
git stash list
Apply stashed changes

sh
Copy code
git stash apply
Drop a stash

sh
Copy code
git stash drop
Remove untracked files

sh
Copy code
git clean -f
Advanced Commands
Rebase a branch onto another

sh
Copy code
git rebase branch-name
Interactively rebase

sh
Copy code
git rebase -i HEAD~n
Cherry-pick a commit

sh
Copy code
git cherry-pick commit-id
View a specific commit

sh
Copy code
git show commit-id
Blame a file to see changes by line

sh
Copy code
git blame filename
These are some of the most commonly used Git commands. Each command has various options that can be used to achieve different results, and you can always refer to the Git documentation or use the git help command for more detailed information.
