# Init

## Brand new proj, hook up with remote repo

```bash
# You have new local project not under version control, this will give you .git folder
git init

# Link it with remote repo
git remote add origin https://github.com/FanrayMedia/git-notes.git

# It's important to have your user info the same as your remote repo, as this will ensure remote repo recognizes the commit author
# Go to your github profile or bitbutcket account settings for full name and email
# Then check out your info for your local repo, or see it globally add "--global"
git config user.name
git config user.email
git config --global user.name
git config --global user.email

# If your global info is inline with github and this repo is for bitbucket, then set these locally
git config user.name "Ray Fan"
git config user.email "my.email.on.bitbucket@gmail.com"

# Now you can stage and commit your initial code
git ca "Initial commit"

# Push to remote repo
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

## Change remote git url

```bash
# sometimes you want to change proj remote repo, say from github to bitbucket
git remote set-url origin new-git-url-here
```
