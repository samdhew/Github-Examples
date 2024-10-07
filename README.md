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
git clone <repo_url>
git clone <repo_url> -b <branch_name>
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

## Remotes

```sh
git remote -v
git remote add "origin" <repo_url>
git remote set-url "origin" <repo_url>
```

## Stashing

## Merging

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