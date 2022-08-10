# GIT & GIT HUB v1.1
### 10/08/22
## WHAT IS VERSION CONTROL
- For lots of files with different version
- For multiple people working at once
- resolving conflict
- otherwise its hard to manage files
- allows us to keep track of who is working on what
- Helps to keep track of large group of files
- Popular Systems: Git, SVN, Mercurial

## GIT
- Version Control System
- Runs locally on your computer
- Open source
- distributed control system, everyone has there copy of the history
- Git works with **repositories** and complete history and version tracking
- each change is bundled up in a **commit** made by an **author**

#### Why Git?
- Creates a history of changes
- allows roll back, everyone to use it and back up.

# First Repo!

## Subheading

This is the first change to this file

a test repo for the git lesson

```bash
ls -la
mk dir foo
```
- one
- two
- three

## GITHUB
- Web-app owned by microsoft
- Wraps useful functionality around git
- A cloud based git system repository
- shared easily online, popular on companies on a paid plan for private repos
- CLI command line interface when we use git
- vs code has a gui for github, but most users use the command line.

## Core Git Concepts <br /> <br />

### Respository
#### A folder where all files are stored
`$ git init`
- respository as a desk with paper and each paper is one of the files you want to keep track of metaphorically 
- Only created once! and files aren't touched from then on. If done again we lose all our previous data. 
- To start a repository <br /> <br />
### Staging Area
`$ git add .`
- git add selects that file, and moves it to the staging are, marking it as the next commit
- root directory on your device with the source files
- Metaphorically a box, files you made changes to and put into the box on the desk. Files you want Git to look over. 
- After adding you wont get any output on terminal
- `git status` is used to see the status of the git, whats commited, changes etc.
- you have to `git add` everytime a change is made
- **Highlighting** the files you want in your repo <br /> <br />
### Commit
`$ git commit -m "message"` 
- A Bookmark where all changes to files in the staging area are stored.
- All the files you have **staged** can be stored or saved
- just type `git commit` brings up nano ctrl O then ctrl X, needs extra parameters by: `git commit -m "Initial commit"`<br /> <br />



## Some Git Terminology and commands

- **working directory**: root directory on your device with the source files > `git add` = **staging**: temp storage for changes in working directory > `git commit` = **local repository**: a repo stored on your laptop/device > `git push` = **remote repository**: a repo stored in a cloud

- **fork** - create your own remotae repo for someone else's with all of the history up to the time of the fork.
- **clone** - copy the contents of a remote repo to your local repo and working directory
- **master**/**main** - the default brach on a repo
- **origin** - the default name of the connection to the remote repo
- `git dif` = to see the changes in repository
- `git commit -am "message"`  = does a .add combined with a commit "-a" = add "=m" = message
- `git log` = to see the changes, latest commit would be the first one.
- `git reset HEAD~1` = goes back 1 commit. Before the commit happened or staged. It requires to me added and committed once again. adding `git reset --hard HEAD-1` does a more permanent change
- The number of HEAD~(number) is the amount of times you want to go back, so if you have 3 commits and you enter (number) as one it will go back one commit.
- it also resets to that HEAD point **permanently**


# Adding Git to GitHub

- select new repository in github
- fill in the repository, change options, select SSH
- go back to your local repo
- `git remote -v` checks if any local repos are connected to github
- `git remote add origin "link to github"` - to add repository to github only done the first time
- `git push -u origin master` < connects local to remote through SSH key, master is the branch name






