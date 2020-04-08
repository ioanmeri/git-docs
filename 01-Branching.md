# Branching

## New Branch

To create a new branch and switch to it at the same time

```
git checkout -b iss53
```

shortcut for:
```
git branch iss53
git checkout iss53
```

## Back to master
switch back to your master branch:

```
git checkout master
```

## Merge a branch

Merge the hotfix branch back into your master branch to deploy to production.

```
git checkout master
git merge hotfix
```

## Delete a branch
```
git branch -d hotfix
```


Source:

[gi-scm.com](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
