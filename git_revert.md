# REVERT

## You want to discard a local change to a file

```bash
git co file_changed # revert that file
git co . # revert all changed files
```

## You want revert a local commit (a commit that you haven't pushed to remote)

```bash
git reset HEAD~1
# On windows use tilda, the number following it is the number of commits you want to reset
```

## You pushed committed changes to origin and you want to revert back

```bash
# You committed and pushed a "Regrettable commit"
git reset --hard HEAD~1
git push origin master --force
# Now by looking at the commit page on origin, the regretable commit is gone from the list
git reflog
# git does not really delete anything, you can still see your regretable commit with reflog 
```
