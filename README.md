git-cheatsheet
==============
A quick reference for before your morning coffee.

* [Basic](./basic/README.md)
* [Branching](#branching)
  * [Create new branch](#create-new-branch)
  * [Switch to a branch](#switch-branch)
  * [Merge branches](#merge-branches)
  * [Delete a branch locally](#delete-branch)
  * [List](#list-branches) 
* Rollback
  * Restore file from a custom commit (in current branch) 
* Tagging with semantic versioning
  * Bower
  * NPM 	
* Set remote
  *  Add remote
  *  Remove remote

#<a id="branching">Branching</a>
###<a id="create-new-branch">Create a new branch</a>
```bash
git checkout -b <name>
```


###<a id="switch-branch">Switch to a branch</a>
```bash
git checkout <name>
```

###<a id="merge-branches">Merge branches</a>
```bash
git checkout <branch to merge to>
git merge --no-ff <branch to merge from>
```

###<a id="delete-branch">Delete a branch locally</a>
```bash
git branch -d <branch name>
```

###<a id="list-branches">List branches</a>
```bash
git branch [-a]
```
`-a` will list both local and remote branches



# <a id="rollback">Rollback</a>

### <a id="restore-file-to-commit">Restore file from a custom commit (in current branch)</a>

```bash
 git checkout 6eb715d -- index.html
```




#<a id="tagging">Tagging with semantic versioning </a>

### <a id="bower">Bower</a>

```bash
bower version patch|minor|major
```

### <a id="npm">NPM</a>

```bash
npm version patch|minor|major
```


# <a id="set-remote">Set Remote</a>

###<a id="add-remote">Add remote URL</a>

```bash
git remote add <name> <address>
#Example: git remote add origin https://github.com/rileyjshaw/git-cheatsheet.git
```

###<a id="remove-remote">Remove remote</a>
```bash
git remote rm <name>
```

