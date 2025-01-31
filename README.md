Git Commands
============

## Translated Versions
- [Versão em português](READMEpt.md)

___

_A list of my commonly used Git commands_

*If you are interested in my Git aliases, have a look at my `.bash_profile`, found here: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |

Everything below is mine (Zubaer)
---

### My Git-Commands 

| Command | Description |
| ------- | ----------- |
|`git remote -v`| Show remote url after name |
|`git remote rm `| Remove the remote named <name> |
|`git branch -a`| Show all branch, example when you pull from a repo that has branches you can use it to show all branches|
|`git branch --list`| Existing branches are listed|
| `git remote update` | Update all branches |
| `git status -u` | Check if GitHub sync with local |
| `git remote rm <name> ` | Remove <name> remote |
| `rm -rf .git` | Remove git file from folder|
|`git branch -d <branchname>`| Remove branch|
|`git remote update` -> `git status -u`| To check if local is in sync with the repository|
|`git log --graph --oneline`| Compresed version of git tree|
|`git log --graph`| Show full git tree in very detail|
|`git checkout <branch-name>`| As the command says, the head will be on the provided name branch|

---

### Comonly used git operation

When cloning: 

```
git clone (provide https link)
```

When doing some changes or uploading new file to the git directory locally and you want to push it to the remote repository

```
git remote update

git status

git pull

git add . 
or
git add [the specific path to that specific file/folder that you have changed or added]

git commit -m "provide-anynmessage"

git push
```
  
When you cloned a repo that has one branch e.g. main and then how to create another branch and then make this branch available on the remote repo also
Assuming you have only one branch - main  
  
```
git checkout -b [branch name]
  
git push (when you do that you will see some instruction on the git-bash, just follow it to the next step)
  
```



