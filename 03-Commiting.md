# Commiting 

## Rewriting the most recent commit message

```
git commit --ammend
```
edit the commit message and
```
ctrl+0
```

to write out changes


## Adding more changes to my last commit

### Without Changing It's Message
```
git add .
git commit --amend --no-edit
```

### Pushing

If you **haven’t pushed** the last commit yet to your remote, **a single push is enough**.

**else**:

```
$ (some_branch) git push -f origin some_branch
```
