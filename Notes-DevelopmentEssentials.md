# GitHub

## cloning repository

`git clone https://github.com/webprogramming260/startup-example.git`
`test`

## making changes

```
 git push
 git add test.md
 git commit -am "update(notes) thoughts about startup applications"
 git push
```


1. Pull the repository's latest changes from GitHub (`git pull`)
2. Make changes to the code
3. Commit the changes (`git commit`)
4. Push the changes to GitHub (`git push`)

`git fetch` lets you check pull latest infor without changing local repository
ex:
```
git fetch
git status
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)
git pull
```

## merge conflicts
if a file has been changed in two different commits that are unsynced (branching) then they will need to be merged
`git pull` will give a conflict warning and then you will need to go in a change the files in question, and then commit and push the changes

## forks
fork lets you copy a public repository 
forks allow you to modify the repository fork and push the changes as a _pull request___
