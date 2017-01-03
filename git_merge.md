# Merge

## Merge by Pull

```bash
# You are at your local branch and you want to pull in a branch named dev from remote
git pull --rebase origin dev

# http://stackoverflow.com/q/7200614/32240
# git pull is basically the same as git fetch; git merge origin/master.
# git pull --rebase is basically the same as git fetch; git rebase origin/master.
```