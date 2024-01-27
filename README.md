# git-cheatsheet

```shell
# Add file/folder to staging area
 git add folder/file/. 

 # Commit a local change
 git commit -m "commit-message-here"

 # Check your current branch
 git branch

 # Get all the branches
 git branch -a

 # Change brach
 git checkout branch-name
 git switch branch-name

 # Create new branch from current branch
 git checkout -b new-branch-name-here
 git switch -c new-branch-name-here

 # Show status
 git status

 # Add and commit in same command
 git commit -am "commit-message-here"

 # Rename current commit message 
 git commit --amend -m "new-commit-message-here"

 # Add additional commits to same message before pushing
 git add .
 git commit --amend --no-edit
 
 # Override remote history
 git push origin branch-name --force
 
 # Revert a commit (creates a new commit that undoes the changes made by            original commit)
 git revert commit-id
 
 # Get commit id or list of commits made
 git log --oneline

 # Stash to stack and retrieve it 
 git stash
 git stash pop

 # Stash in a dedicated space (here stash-name is the unique namespace)
 git stash save stash-name

 # Get all the stashes
 git stash list
 
 # Apply a specific stash (where 0 is the index of the stash, refer prev command)
 git stash apply 0

 # Rename branch (renames current branch to main)
 git branch -M main

 # Decorate the logs
 git log --graph --decorate --oneline -all
 
 # Switch to previous branch
 git checkout -
 
 # Override local changes with remote changes
 git fetch origin
 git reset --hard origin/branch-name-here

 # Remove untracked files
 git clean -df
 
 # Using git diff command
 git diff HEAD <file_name>
 git diff <file_name>
 git diff --staged <file_name> or  git diff --cached <file_name>
 git diff <branch_name1> <branch_name2> <file_name>
 git diff <commit_hash> <commit_hash> <file_name>

# Rebase current branch to another branch
git rebase another-branch-name-here

# Squash, reword etc.. to commits
git rebase -i HEAD~n

# Add tags
# Read about tags (https://git-scm.com/book/en/v2/Git-Basics-Tagging)

# Create a git alias
git config --global alias.aliasName 'original command or custom command'

```