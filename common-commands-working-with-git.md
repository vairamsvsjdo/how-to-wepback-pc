software required:

```
git-scm installed
vscode installed
.net sdk 2.0 installed
nodejs latest (not LTS)
angular-cli
yarn
webpack 
```

create a pull request, rebase before performing pull request. git clone, git remote add upstream, git pull, git checkout, git add, git commit, git commit, git pull, git rebase, git merge, git push upstream, 
```
git branch new-branch
```

```
git master
```
```
git dev
```
```
git checkout dev-fix1
```
```
git checkout dev-feature-a
```



creating and switch to a new branch:

```
git checkout -b new-branch
```

```
git checkout master
```

```
echo "hello world" > mynewfile.txt
```

```
git add -A  
```
or 
```
git add mynewfile.txt
```

```
git commit -m "fixes #1 new commit"
```

```
git commit
```

```
git config --global core.editor "nano"
```
Or vim:
```
git config --global core.editor "vim"
```

```
git status
```
Depending on the changes that you have made, you will receive output that looks something like this:

```
git push --set-upstream origin new-branch
```

Update Local Repository
```
git remote -v
```

Output
origin  https://github.com/jaydevops/angular-cli.git (fetch)
origin  https://github.com/jaydevops/angular-cli.git (push)

```
git remote add upstream https://github.com/angular-cli/angular-cli.git
```

```
git remote -v
```

output seen below
origin  https://github.com/jaydevops/angular-cli.git (fetch)
origin  https://github.com/jaydevops/angular-cli.git (push)
upstream    https://github.com/angular/angular-cli.git (fetch)
upstream    https://github.com/angular/angular-cli.git (push)


```
git fetch upstream
```

```
git checkout master
```

```
git merge upstream/master
```

rebase and update a pull request, squash commits, update comments

```
git fetch upstream
```
```
git log
```
```
git log --author=your-username
```


the number of commits since you started working:

```
git rebase -i HEAD~x
```

```
git merge-base new-branch master
```

returns a commit hash example: 0f83552034f9c14694ee6e5c8771a30a536b6d9f

```
git rebase -i 0f83552034f9c14694ee6e5c8771a30a536b6d9f
```

Squash Commits
```
pick 24fd2ac fixes #1
squash 63cd747 additional changes forgot to check in
```

```
:wq
```


```
git rebase -i 0f83552034f9c14694ee6e5c8771a30a536b6d9f
```

change comments
```
reword 24fd2ac fixes #1 - additional comment added 
```

```
:wq
```

Complete the Rebase

```
git rebase upstream/master
```

```
git rebase --continue 
```

Update Pull Request with Force-Push

```
git config --global push.default simple
```

```
git checkout new-branch
```

```
git push -f
```


get deleted Commits as long as you maintain .git folder historically on your local machine.


```
git reflog
```

```
git checkout -b new-new-branch a1f29a6
```

```
git checkout master
```
https://git-scm.com/book/en/v2/Git-Branching-Rebasing

```
git pull --rebase upstream master
```


```
git push -f origin master
```


```
git branch -d new-branch
```

```
git push origin --delete new-branch
```
