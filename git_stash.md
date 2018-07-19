# Stash

https://www.atlassian.com/git/tutorials/saving-changes/git-stash

You have made changes to your current branch, then you want to create a new branch and move these changes over

```bash
# say currently I'm on dev branch
git stash

# now dev is clean you are free to checkout new-branch
git co new-branch

# now you are on the new branch, pop the changes out
git stash pop
```