# Counting

## Get Total lines of code in a git

```
git ls-files | xargs wc -l
```

Exlcude files like package-lock.json
```
git ls-files | grep -v -E "\lock.json$" |  xargs wc -ls
```