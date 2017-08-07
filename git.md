# Ignoring an already checked-in directory
```
git rm -r --cached <your directory>
```
The -r option causes the removal of all files under your directory.
The --cached option causes the files to only be removed from git's index, not your working copy. By default git rm <file> would delete <file>

# push a new local branch to a remote Git repository and track it
```
git checkout -b <branch>  | git branch <branch>
git push -u origin <branch>
```

# Adding Only Untracked Files

git add -i. Type a (for "add untracked"), then * (for "all"), then q (to quit)


# discard all Changes not staged for commit
git checkout -- .





