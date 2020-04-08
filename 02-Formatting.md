# Format Commits

## Show today's commits
```
git log --since="6am"
```

## After a specific day
```
git log --after=dec17
```

## For a specific day
```
git log --after=jun9 --before=jun10
```

w/ author
```
git log --since=jun9 --until=jun10 --author=Robert 
```

The --since/--after and --until/--before parameters can also take stuff like 3 days ago, yesterday, etc.
```
git log --since=yesterday
```

##  Print only titles & part of their hash
```
git log --oneline
```
Output: 

fba63d5 add profile nav component
f2115fc profile page layout
34d4994 add Profile route



## Reverse Order
```
git log --reverse
```
Note that .e.g. `git log -10 --reverse` would get 10 **last** commits then reverse list
