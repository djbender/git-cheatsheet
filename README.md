# git-cheatsheet

## Sleuthing

### Which branches contain \<commit\>?

    git branch --contains <commit>
    git branch -r --contains <commit>
    git branch -a --contains <commit>

### What are commits between `branch` and `master`?

     git log origin/master..branch --oneline
     
As a pretty graph with color!

    git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%Creset' --abbrev-commit --date=relative master..branch
