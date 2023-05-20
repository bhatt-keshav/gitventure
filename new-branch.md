Create a new branch based on an existing branch (master) by:

```
git switch -c new-branch master
```
the switch c is for create

but this `new-branch` has been created locally, it doesn't have a branch on the remote to track it. Therefore do

```
git push -u origin new-branch
```

the -u flag is is equivalent to `git push --set-upstream origin new-branch`

> if you add the -u flag—Git will set origin/solaris as the upstream for your current branch if (and only if) the push succeeds. 
So you should supply -u on the first push. In fact, you can supply it on any later push, and it will set or change the upstream at that point. 
But I think git branch --set-upstream-to is easier, if you forgot.


cf. https://stackoverflow.com/questions/37770467/why-do-i-have-to-git-push-set-upstream-origin-branch
