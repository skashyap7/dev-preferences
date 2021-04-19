

## Useful git commands

1. Checkout code at specific version
```
 git log
 git checkout <SHA1>
```

2. Checkout only specific file/s from a branch to another 
```
  git checkout <source_branch> -- <filename>
```

3. Reset the local branch with pushing it upstream
```
git reset --hard <commit>
git push --force origin branch
```

4. Git Cherry pick a change
```
git cherry-pick <commit>

If you notice bad object errors, make sure local is synced with remote by use

git fetch --all 
```

5. Set reference for current branch and use that for pushing

Set in your bashrc
```
alias cb="git symbolic-ref --short HEAD"
alias gpo='git push origin "$(git symbolic-ref --short HEAD)"'
```
When pushing code to remote use
``` 
 gpo
```
