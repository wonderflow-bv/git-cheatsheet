git-cheatsheet (basic)
==============

#Basic actions
###Add file to staging area (preparing for a commit)
```bash
git add <list of files>
git add .  #stage changed or new files in working tree (does not stage 'rm' actions)
git add -u  #stage changed or removed files (does not stage untracked files)
git add [--all|-A]  #shortcut for doing both git add . and git add -u
git add *.css  #add all .css files in current directory to tracked files
git add "*.css"  #add all css files in entire project to tracked files
```

###Remove a file from staging area
```bash
git rm <list of files>  #untracks *and removes* files
git rm <list of files> -cached  #untracks files but doesn't remove them. Usually want to add these to .gitignore
```

###Record a snapshot of the staging area via a commit
```bash
git commit -m "<commit message>"
git commit -am "<commit message>"  #useful shorthand to automatically stage all tracked, modified files before the commit
```
_**Note:** Commit messages should be brief, and written in the present tense._
>"Add PWM block for motor 2"

###Push all unsynced commits to a remote repository
```bash
git push [-u] <remote repository name> <local branch name>
#Example: git push -u origin master
```
`-u` sets the upstream repository to the specified remote. After this, you can run `git push`, `git fetch` etc without having to specify remote and branch names.




#Basic references
```bash
git status  #Check what has changed since the last commit
git diff  #Show unstaged line differences since last commit
git diff --staged  #Show staged line differences
git diff <file name>  #Show changes in a specific file since last commit
git diff <commit id> <commit id>  #Show changes between two commits
git log  #Show repository history
git blame <file name>  #Show what revision and author last modified each line of a file
```

#Terminology
 - __master__ : default branch
 - __origin__ : conventional name for the default upstream repo
 - __HEAD__ : latest (or currently checked-out) commit
 - _[More...](http://stackoverflow.com/questions/7076164/terminology-used-by-git)_


#<a id="refs"></a>Useful references
 - From terminal: `git help <command>` (alternatively, check out the [git(1) Manual Page](https://www.kernel.org/pub/software/scm/git/docs/))
 - [Git Reference](http://gitref.org/)
 - [Everyday Git](https://www.kernel.org/pub/software/scm/git/docs/everyday.html)
 - [Pro Git](http://git-scm.com/book)
 - Codeschool courses: [1](https://www.codeschool.com/courses/try-git), [2](https://www.codeschool.com/courses/git-real), and [3](https://www.codeschool.com/courses/git-real-2)
