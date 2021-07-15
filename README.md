# git-cheatsheet
Collection of git tips / commands / docs to keep them in one accessible place.

## 1. Git Config
#### Define the author name and author email to be used for all commits by the current user.
```
git config --global user.name <name>
git config --global user.email <email>
```

## 2. Start Project
#### Create empty Git repo in specified directory.
```
git init <directory>
```
#### Clone repo located at <repo> onto local machine.
```
git clone <repo>
```

## 3. Daily Activity
#### Displays the status of your working directory.
```
git status
```
#### Stage all changes in <directory> for the next commit.
```
git add <directory>
```
#### Commit the staged snapshot
```
git commit -m "<message>"
```
#### Display the entire commit history.
```
git log
```
#### Show unstaged changes between your index and working directory.
```
git diff
```


## 4. Revert Changes
#### Create new commit that undoes all of the changes made in <commit>, then apply it to the current branch.
```
git revert <commit>
```
#### Reset staging area to match most recent commit.
```
git reset 
```
#### Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.
```
git reset --hard
```

## 5. Git Branching
#### List all local branches in repository. With -a: show all branches (with remote).
```
git branch -a
```
#### Create and check out a new branch named <branch>.
```
git checkout -b <branch>
```
#### Merge <branch> into the current branch.
```
git merge <branch>
```

## 6. Git Rebase
#### Interactively rebase current branch onto <base>. Launches editor to enter commands for how each commit will be transferred to the new base.
```
git rebase -i <base>
```

## 7. Tagging
#### List all tags.
```
git tag
```
#### Create a tag reference named name for current commit. Add commit sha to tag a specific commit instead of current one.
```
git tag <name> <commit sha>
```

## 8. Synchronizing Repositories
#### Fetch changes from the remote, but not update tracking branches.
```
git fetch
```
#### Fetch changes from the remote and merge current branch with its upstream.
```
git pull
```
#### Push local changes to the remote. Use --tags to push tags.
```
git push [--tags]
```

---
CI Robots
[@dwsclass](https://github.com/dwsclass) dws-dev-004-git
  
---
License: [APACHE LICENSE, VERSION2.0](https://www.apache.org/licenses/LICENSE-2.0)
