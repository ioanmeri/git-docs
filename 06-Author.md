# Git Author

## Find out the author
```
git config --list
```

## Change author of all commits

One liner, but be careful if you have a multi-user repository - this will change all commits to have the same (new) author and committer.

```
git filter-branch -f --env-filter "GIT_AUTHOR_NAME='Newname'; GIT_AUTHOR_EMAIL='new@email'; GIT_COMMITTER_NAME='Newname'; GIT_COMMITTER_EMAIL='new@email';" HEAD
```

if already pushed then
```
git push origin master -f
```