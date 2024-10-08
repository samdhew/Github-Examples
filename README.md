# Github-Examples
A repo containing GitHub for programmatic examples

## Git Hidden Folder
There is a hidden folder called `.git` which tells that the project is a git repo

## Initialization

```sh
git init
```

## Cloning
There are 3 ways to clone: HTTPS, SSH & GitHub CLI

### HTTPS

```sh
git clone https://github.com/<username>/<repo_name>.git
git clone https://github.com/<username>/<repo_name>.git -b <branch_name>
```

### SSH

```sh
ssh-keygen -t rsa
# Add SSH public key to github.com to authenticate via SSH 
# github.com ==> settings ==> SSH and GPG keys ==> SSH Keys ==> New SSH Key ==> Authentication Key 
eval 'ssh-agent'
ssh-add <ssh_private_key_path>
ssh -T git@github.com
```

```sh
git clone git@github.com:<username>/<repo_name>.git
git clone git@github.com:<username>/<repo_name>.git -b <branch_name>
```

### GitHub CLI

```sh
gh auth login
gh repo clone <username>/<repo_name>
gh repo clone <username>/<repo_name> -b <branch_name>
```

## Status
Shows what files will or will not be commited

```sh
git status
```

## Commits
Commits staged changes to be pushed to remote origin

```sh
git commit -m "commit message"
git commit -a -m "commit message"
```

## Pull
Pulls remote origin to local repo

```sh
git pull origin main
```

## Push
Pushes local repo to remote origin

```sh
git push -u origin main
```

## Branches

List local branches
```sh
git branch
```

List remote branches
```sh
git branch -r
```

List local and remote branches
```sh
git branch -a
git branch -l 'feature/*'
```

Print current branch
```sh
git branch --show-current
```

Change current branch
```sh
git checkout <branch_name>
```

Create new branch
```sh
git branch <new_branch_name>
```

Create new branch and change
```sh
git checkout -b <new_branch_name>
```

Delete existing branch
```sh
git branch -d <branch_name>
git branch -D <branch_name>
```

Rename branch
```sh
git branch -m <new_branch_name>
git branch -m <old_branch_name> <new_branch_name>
```

Copy branch
```sh
git branch -c <new_branch_name>
git branch -c <old_branch_name> <new_branch_name>
```

## Remotes

```sh
git remote -v
git remote add "origin" https://github.com/<username>/<repo_name>.git
git remote set-url "origin" https://github.com/<username>/<repo_name>.git
```

## Stashing

Stash current changes (Keep a side for time being)
```sh
git add .
git stash
```

List stashed changes
```sh
git stash list
```

Pop stashed changes (Bring back)
```sh
git stash pop
```

## Merging
Merges one branch to another

```sh
git merge main
```

## Add
Adds changed files to stage

```sh
git add README.md
git add .
```

## Reset
Moves staged changes to unstaged

```sh
git reset
```

## Log
Shows recent commits

```sh
git log
```