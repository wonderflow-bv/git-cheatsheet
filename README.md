git-cheatsheet
==============
A quick reference for before your morning coffee.

* [Basic](./basic/README.md)
* [Branching](#branching)
  * Create new branch
  * Switch to a branch
  * Merge branches
  * Delete a branch locally
  * List 
* Rollback
  * Restore file from a custom commit (in current branch) 
* Tagging with semantic versioning
  * Bower
  * NPM 	
* Set remote
  *  Add remote
  *  Remove remote

#<a id="branching">Branching</a>
###Create a new branch
```bash
git checout -b <name>
```


###Switch to a branch
```bash
git checkout <name>
```

###Merge branches
```bash
git checkout <branch to merge to>
git merge --no-ff <branch to merge from>
```

###Delete a branch locally
```bash
git branch -d <branch name>
```

###List branches
```bash
git branch [-a]
```
`-a` will list both local and remote branches



# Rollback

### Restore file from a custom commit (in current branch)

```bash
 git checkout 6eb715d -- index.html
```




#Tagging with semantic versioning 

### Bower

```bash
bower version patch|minor|major
```

### NPM

```bash
npm version patch|minor|major
```


# Set Remote

###Add remote URL

```bash
git remote add <name> <address>
#Example: git remote add origin https://github.com/rileyjshaw/git-cheatsheet.git
```

###Remove remote
```bash
git remote rm <name>
```

