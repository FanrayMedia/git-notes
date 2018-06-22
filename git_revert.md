# REVERT

## Undo changes

```bash
# You made changes to a file, you haven't staged or committed
git co file_changed # revert that file
git co . # revert all changed files
```

## Un-stage

```bash
git add dir/a.txt # to stage
git reset HEAD dir/a.txt # to unstage
```

## Un-commit local commit (a commit that you haven't pushed to remote)

```bash
git ca "Commit some files" # to commit
git reset HEAD~1 # On windows use tilda, un-commit the last number of commits
```

## Un-commit changes you pushed origin

```bash
# You committed and pushed a "Regrettable commit"
git reset --hard HEAD~1
git push origin master --force
# Now by looking at the commit page on origin, the regretable commit is gone from the list
git reflog
# git does not really delete anything, you can still see your regretable commit with reflog 
```
## How do I “un-revert” a reverted Git commit?
https://stackoverflow.com/a/8730046/32240

If you haven't pushed that change yet, `git reset --hard HEAD^`
