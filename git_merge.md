# Merge

## When merge from featured branch to dev "Squash and merge" should be used

[Squash and merge](https://help.github.com/articles/about-pull-request-merges/#squash-and-merge-your-pull-request-commits) will make your dev and master tidy.

Afterward you may experience [The branch 'x' is not fully merged](https://stackoverflow.com/questions/7548926/git-and-the-branch-x-is-not-fully-merged-error) warning which is not error, you can do force delete to remove the featured branch.

## Merge by Pull

```bash
# You are at your local branch and you want to pull in a branch named dev from remote
git pull --rebase origin dev

# http://stackoverflow.com/q/7200614/32240
# git pull is basically the same as git fetch; git merge origin/master.
# git pull --rebase is basically the same as git fetch; git rebase origin/master.
```
