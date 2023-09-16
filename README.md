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
  * [Delete Commit History](#delete-commit-history)
  * [Change Git Remote URL](#change-git-remote-url)
  * [Create Requirements.txt](#create-requirements.txt)
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
git init
git add .
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

#### Delete Commit History

This Git command deletes the commit history of a repository on GitHub.

```
Step1: Create a new branch
Step2: Add all the files
Step3: Commit the changes
Step4: Delete the branch
Step5: Rename the current branch to main
Step6: Force update your repository
```

```
git checkout --orphan latest_branch
git add .
git commit -m "<MESSAGE>"
git branch -D main
git branch -m main
git push -f origin main
```

#### Change Git Remote URL

This Git command changes the URL of a Git remote.

```
git remote set-url origin https://github.com/<USER>/<REPO-NAME>.git
```

To verify that the changes were made use the 'git remote' command with the '-v' option (verbose).

```
git remote -v
```

#### Create Requirements.txt

This command uses Pipreqs to create a requirements.txt file

```
python -m pipreqs.pipreqs
```

## Credits

Everything is coded by Alex lo Storto

Licensed under the MIT License.
