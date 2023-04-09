<h1 align="center">Git Commands</h1>

This is a repo which contains the Git commands I use most frequently.

## Table of Contents

<details>
  <summary>Click to expand</summary>
  
- [Commands](#commands)
  * [Stage Changes](#stage-changes)
  * [Commit Staged Changes](#commit-staged-changes)
  * [Push Commits](#push-commits)
  * [Undo Previous Commit](#undo-previous-commit)
  * [Rename Folder when Cloning](#rename-folder-when-cloning)
- [Credits](#credits)
</details>

## Commands

#### Stage Changes

This Git command stages any modified files.

```
git add .
```

#### Commit Staged Changes

This Git command commits any staged changes.

```
git commit -m "<MESSAGE>"
```

#### Push Commits

This Git command pushes all commits to the remote repository.

```
git commit -m "<MESSAGE>"
```

#### Undo Previous Commit

This Git command undoes the previous commit if it has not been pushed yet.

```
git reset --soft HEAD~
```

#### Create Repo

This Git command creates a local repository on the command line.

```
git add .
git init
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/alexlostorto/<REPO-NAME>.git
git push -u origin main
```

#### FATAL: No Upstream Branch

This Git command fixes the 'fatal: The current branch main has no upstream branch.' error.

```
git config --global push.autoSetupRemote true
git push
```

#### Rename Folder when Cloning

This Git command changes the name of the folder when cloning from GitHub.

```
git clone <Repo> <DestinationDirectory>
```

## Credits

Everything is coded by Alex lo Storto

Licensed under the MIT License.
