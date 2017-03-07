# git-commands
Frequently used git commands

# initialize git
git init

# see what you have changed since the last commit
git diff

# stage files for committing
git add .

# commit changes
git commit -m "Made some changes"

# create a branch and switch to it
git checkout -b issue87

# list branches
git branch

# switch to a different branch
git checkout issue13

# change remote 
git remote remove origin

git remote add origin https:#github.com/dancancro/ng2-redux-form

# save changes without committing them so you can go to a different branch and come back later
git stash

# restore stashed changes
git stash apply

# push the current branch to the same name on the remote
git push origin HEAD

# compare two branches
git diff branch1..branch2

# delete a local branch
git branch -d branchname

# delete a remote branch
git push origin --delete branchname

# merge a branch into another branch
git checkout dest_branch

git merge source_branch

# discard all unstaged changes in the current branch
git checkout -- .

# Remove untracked files from the working tree
git clean -xfd

# [Create a new branch with changes](http://stackoverflow.com/questions/3899627/create-git-branch-with-current-changes)
git branch mynewbranch
git git reset --soft HEAD~3 # only if you want to undo last 3 commits
git checkout mynewbranch

# Undo last commit without undoing the changes. Do this so you can see the differences 
# between your files and a previous commit. Repeat the command until you reach the point
# against which you want to compare your current files 
git reset --soft HEAD~

# [Combine commits from a branch and merge it into another branch](http://stackoverflow.com/questions/5308816/how-to-use-git-merge-squash)
git checkout master
git merge --squash bugfix
git commit


# Useful articles

[Writing a good commit message](https://chris.beams.io/posts/git-commit/)
[Set of useful commands like this but much better](https://www.atlassian.com/git/tutorials/rewriting-history)
