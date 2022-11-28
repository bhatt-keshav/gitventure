To change commit message of unstaged changes do

```
git commit --amend -m "your new message"
```

The `-m` flag will change your commit message directly in the terminal without having to use the inbuilt text editor, which if `vim` is unexitable.

Then just perform `git push` to push your changes. 

However, if the files have been committed then apply the same `--ammend` command, but also do:

```
git push <remote> <branch> --force
# Or
git push <remote> <branch> -f
```

