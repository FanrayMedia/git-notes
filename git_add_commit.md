# Add & Commit

## Add all and Commit with message

```bash
git add -A && git cm "Commit all new, updated and deleted files"

# Note "git commit -Am" is not valid
```

## Add

```bash
git add -A # stages All, is equivalent to "git add .; git add -u"
git add .  # stages new and modified, without deleted
git add -u # stages modified and deleted, without new
git add *.html # add all files with a given extension, asterisk as a wildcard

# Note "git add -a" is not valid, it must be "git add -A"
```

## Misc

```bash
# Add & Commit modified and deleted files

# You modified a.txt and added new file b.txt
# the following will add and commit a.txt but not b.txt
git commit -am "Updated a.txt"

# Note: I like to keep add and commit as separate actions though this short hand is popular
```