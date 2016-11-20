# Init

## Initialize proj, initial commit, push to github

```bash
# You have local project
git init
git ca "Initial commit"
# You created a repo on github
git remote add origin https://github.com/FanrayMedia/git-notes.git
git push -u origin master
```

## Show remote origin

```bash
git remote show origin # http://stackoverflow.com/a/4089452/32240
```

## When you push to remote, to avoid being asked for credential every time

```bash
# https://help.github.com/articles/caching-your-github-password-in-git/
git config --global credential.helper wincred
```