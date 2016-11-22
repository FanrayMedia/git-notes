# Add & Commit

## Add all and Commit with message

```bash
git ca "Commit all new, updated and deleted files"

# The above is a shortcut for
# Note "git commit -Am" is not valid
git add -A && git commit -m "Commit all new, updated and deleted files"
```

## Add

```bash
git add -A # stages All, is equivalent to "git add .; git add -u"
git add .  # stages new and modified, without deleted
git add -u # stages modified and deleted, without new
git add *.html # add all files with a given extension, asterisk as a wildcard

# Note "git add -a" is not valid, it must be "git add -A"
```

## Show

```bash
# To see the content of a particular commit
git show 3e1508a # commit hash
```

## Misc

```bash
# Add & Commit modified and deleted files

# You modified a.txt and added new file b.txt
# the following will add and commit a.txt but not b.txt
git commit -am "Updated a.txt"

# Note: I like to keep add and commit as separate actions though this short hand is popular
```