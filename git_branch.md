# Branch

## Create local branch

```bash
# Create a local branch "dev" and check it out in one shot
# Alternatively you can do "git br dev", "git co dev"
# The current branch you are on will be the branch "dev" branches off from
$ git co -b dev
$ git push -u origin dev
```

## Delete local branch

```bash
# Delete local branch
# First make sure you are not on the branch to be deleted
git br -d <branch>
git br -D <branch> # Force delete un-merged branches
```

## Delete remote branch

```bash
git push origin :<branch>          # Git versions older than 1.7.0
git push origin --delete <branch>  # Git version 1.7.0 or newer
```

## Bring remote branch to local

```bash
# You created a branch named "dev" on github
$ git fetch
$ git co dev # $ git co -t origin/dev
```

## Refresh the local list of remote branches

```bash
# https://stackoverflow.com/a/36358502/32240
git remote update origin --prune
```

## Show remote info

`git remote -v` can show you both your origin and upstream (if you forked from a repo) info
