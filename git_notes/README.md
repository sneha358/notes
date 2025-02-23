## GIT Notes
__1.__ **change default branch name after git init**
```bash
$ git config set --global init.defaultBranch main
```

__2.__ **Change default branch name even after git init** 
```bash
$ git branch -m master main
```

### BRANCH
__3.__ **To create a branch**
```bash
$ git switch -c name
```
```bash
sneha_ubutu (main) git-example-repo $ git switch -c temp
Switched to a new branch 'temp'
sneha_ubutu (temp) git-example-repo $ git status
On branch temp
nothing to commit, working tree clean
```

__4.__ **To delete any branch**
```bash
git branch -d name
```

```bash
sneha_ubutu (main) git-example-repo $ git branch -d temp
Deleted branch temp (was cd1bf77).
sneha_ubutu (main) git-example-repo $ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

__5.__ **To switch between branches**
```bash
git switch main
```

### staged unstaged commit changes
__6.__ **To add into file**
```bash
$ vim hello.py
```

__7.__ **To check what are the changes before staging**
```bash
$ git diff
```

__8.__ **To staged chages**
```bash
$ git add hello.py 
```

__9.__ **To commit a staged change**
```bash
$ git commit -m "comment"
```

__10.__ **To check what is added after a file is staged**
```bash
$ git diff --staged
```

__11.__ **To unstaged a file staged file**
```bash
$ git restore --staged hello.py
```
