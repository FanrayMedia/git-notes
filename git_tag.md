# Tags

```bash
git tag # display all Tags
git show v1.0.0 # show a specific tag

git tag -a v1.0.0 -m "Initial Release" # add an annotated tag (recommend for tags you are going to keep)
git tag v1.0.0 # add a lightweight tag (no information is stored)

git push origin --tags # push all tags to remote that are not there yet
git push origin v1.0.0 # push specific tag to remote

git tag -d v1.0.0 # delete a local tag
git push origin :refs/tags/v1.0.0 # delete the tag from remote
```