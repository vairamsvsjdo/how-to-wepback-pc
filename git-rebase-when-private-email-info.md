# If you have created commits with private email address

when git rembase -i below displays the file edit is displayed, write for all commits that need replaced wit a line entry 

pick {commitID} message

```` bash
git config --global user.email "replaceemailidfoundingitsettings@users.noreply.github.com"
git rebase -i
git commit --amend --reset-author
git rebase --continue
git push
```
