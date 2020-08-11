# Git Author

## Find out the author
```
git config --list
```

### Repository-specific authors
```
git config user.name "Ioannis Merianos"
git config user.email "ioannismeri@gmail.com"
```

## Change author of all commits

One liner, but be careful if you have a multi-user repository - this will change all commits to have the same (new) author and committer.

```
git filter-branch -f --env-filter "GIT_AUTHOR_NAME='Ioannis Merianos'; GIT_AUTHOR_EMAIL='ioannismeri@gmail.com'; GIT_COMMITTER_NAME='Ioannis Merianos'; GIT_COMMITTER_EMAIL='ioannismeri@gmail.com';" HEAD
```

if already pushed then
```
git push origin master -f
```

