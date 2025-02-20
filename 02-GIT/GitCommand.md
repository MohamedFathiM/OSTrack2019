# بسم الله الرحمن الرحيم

[TOC]

## Git Commands

### Syntax

`$ git <options> command <options>`

### Install

`sudo apt install git`

### Configuration

- URL: <https://www.atlassian.com/git/tutorials/setting-up-a-repository>
- `git config --global user.name 'Your name'`
- `git config --global user.email your@domain.tld`


|Command        |Description                            |URL        |
|-----------------------|---------------------------------------------------------------|---------------|
|`git`            |To ensure that git is installed                                |        |
|`git init`             |Create an empty Git repository or reinitialize an existing one |<https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-init>|
|`git clone`|clone the repository into a new repo |<https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone>|
|`git config`| is a convenience function that is used to set Git configuration values on a global or local project level|<https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config>|
|`git status` | displays the state of the working directory and the staging area|Show the working tree status|
|`git add` |change in the working directory to the staging area.|<https://www.atlassian.com/git/tutorials/saving-changes>|
|`git add .`|add all files to staging area | <https://www.atlassian.com/git/tutorials/saving-changes>
|`git reset` |Reset current HEAD to the specified state|<https://www.atlassian.com/git/tutorials/undoing-changes/git-reset>|
|`git reset HEAD^`|to reset last commit |<https://www.atlassian.com/git/tutorials/undoing-changes/git-reset>|
|`git rm` |The git rm command can be used to remove individual files or a collection of files|<https://www.atlassian.com/git/tutorials/undoing-changes/git-rm>|
|`git commit` |Record changes to the repository |<https://www.atlassian.com/git/tutorials/saving-changes/git-commit>|
|`git diff` |Show changes between commits, commit and working tree, etc|<https://www.atlassian.com/git/tutorials/saving-changes/git-diff>|
|`git stash`|Stash the changes in a dirty working directory away|<https://www.atlassian.com/git/tutorials/saving-changes/git-stash>|
|`git show` |Show various types of objects| |
|`git log` | Show commit logs|<https://www.atlassian.com/git/tutorials/git-log>|
|`git banch -l` |list branch names | <https://www.atlassian.com/git/tutorials/using-branches>|
|`git branch <branch>` |create new branch | <https://www.atlassian.com/git/tutorials/using-branches>|
|`git branch -r` |remote branches | |
|`git branch -d <branch name>`|to delete branch |<https://www.atlassian.com/git/tutorials/using-branches>|
|`git tag -l`|list tag names |<https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-tag>|
|`git tag -e <tag name> <sha for commit>`|force edit of tag message| |
|`git checkout <branch name>` |lets you navigate between the branches created by git branch. | <https://www.atlassian.com/git/tutorials/using-branches/git-checkout>|
|`git checkout -b <branch name>` |create new branch and set head on it | <https://www.atlassian.com/git/tutorials/using-branches/git-checkout>|
|`git merge` |to join two or more development histories together|<https://www.atlassian.com/git/tutorials/using-branches/git-merge>|
|`git rebase`|Reapply commits on top of another base tip|<https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase>|
|`git pull`|The git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content. |<https://www.atlassian.com/git/tutorials/syncing/git-pull>|
|`git push`|Update remote refs along with associated objects|<https://www.atlassian.com/git/tutorials/syncing/git-push>|
|`git remote`|The git remote command lets you create, view, and delete connections to other repositories. |https://www.atlassian.com/git/tutorials/syncing|
|`git remote -v`|List the remote connections you have to other repositories.|-|
|`git push --tags`|The --tags flag sends all of your local tags to the remote repository.|https://www.atlassian.com/git/tutorials/syncing/git-push|
|`git tag -d <tag name >`|to delete tag from local repo  | - |
|`git push :<tag name>` | to delete tag from remote repo | - | 


----------------------------------------------------------------------------------------------------------------------------
### Note : <br>
#### How to sync your fork : <br>
1. open terminal and change directory to your working repo . <br>
2. Create a new connection with remote repo : 
    * `git remote add upstream <URL for original(remote) repo >` 
3. list your remote repo [must remote repo 'upstream' in the list] :
    * `git remote -v`
3. Fetsh the updates 
    * `git fetsh upstream ` 
4. Merge the changes to your master 
    * `git merge upstream/master`
5. Push updates to your fork 
    * `git push origin master`
#### video : https://www.youtube.com/watch?v=-zvHQXnBO6c