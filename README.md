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

# save changes without committing them so you can go to a different 
# branch and come back later
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

# deploy to Heroku
go into your heroku app's 'config' tab (if using the heroku dashboard) and set the NPM_CONFIG_PRODUCTION env var to false
