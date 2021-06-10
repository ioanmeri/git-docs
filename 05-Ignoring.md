# Ignoring

> touch .gitignore # Root directory of the app


## Cleaning Ignored Files

In three steps, you can clean up your repository and make sure your ignored items are indeed ignored:

* Remove the files from the index (not the actual files in the working copy)
```
git rm -r --cached .
```

* Add these removals to the Staging Area...
```
git add .
```

* ...and commit them!
```
git commit -m "Clean up ignored files"
```

## Keep Subfolder
```
src/*
!src/app
```

## Keep 2nd Level Subfolder

```
src/*
!src/vendor
src/vendor/*
!src/vendor/scandipwa
```

