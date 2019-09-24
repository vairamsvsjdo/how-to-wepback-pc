# If you have created commits with private email address
```` bash
git config --global user.email "replaceemailidfoundingitsettings@users.noreply.github.com"
git rebase -i
git commit --amend --reset-author
git rebase --continue
git push
```
