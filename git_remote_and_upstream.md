# git remote

Fork a repo and then add it as upstream

```bash
git remote add upstream https://github.com/repo/i-just-forked.git
```

Verify

```bash
git remtoe -v
```

Pull latest from upstream

```bash
git fetch upstream
```

Merge the dev branch of the just pulled upstream to your chosen local branch

```bash
git merge upstream/dev
```