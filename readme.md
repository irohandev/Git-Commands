# Git Commands Cheat Sheet

A comprehensive list of Git commands with descriptions for easy reference.

## 1. Basic Git Commands

- **`git init`**: Initializes a new Git repository in the current directory.
- **`git clone [repository-url]`**: Copies a Git repository from a remote source (like GitHub) to your local machine.
- **`git add [file-name]`**: Stages a specific file or files to be committed. You can use `git add .` to stage all changes.
- **`git commit -m "[message]"`**: Commits the staged changes to the repository with a descriptive commit message.
- **`git status`**: Displays the status of changes as untracked, modified, or staged.
- **`git log`**: Shows the commit history, listing all past commits.
- **`git diff`**: Displays differences between various commits, or between the working directory and the last commit.

## 2. Branching and Merging

- **`git branch`**: Lists all local branches in the repository. The current branch is highlighted with an asterisk `*`.
- **`git branch [branch-name]`**: Creates a new branch with the specified name.
- **`git checkout [branch-name]`**: Switches to the specified branch.
- **`git checkout -b [branch-name]`**: Creates a new branch and switches to it.
- **`git merge [branch-name]`**: Merges the specified branch into the current branch.
- **`git branch -d [branch-name]`**: Deletes the specified branch locally.

## 3. Remote Repositories

- **`git remote -v`**: Lists all remote repositories linked to the local repository.
- **`git remote add [name] [url]`**: Adds a new remote repository.
- **`git pull [remote] [branch]`**: Fetches and integrates changes from a remote branch into the current branch.
- **`git push [remote] [branch]`**: Pushes the committed changes from the local branch to the specified remote branch.
- **`git fetch [remote]`**: Downloads objects and references from another repository.
- **`git remote rm [name]`**: Removes the specified remote repository.

## 4. Undoing Changes

- **`git reset [commit]`**: Resets the current branch to a specified commit. Use `--hard` to discard all changes after the specified commit or `--soft` to keep them staged.
- **`git revert [commit]`**: Creates a new commit that undoes the changes from the specified commit.
- **`git checkout -- [file-name]`**: Discards changes in the working directory for a specific file.
- **`git clean -f`**: Removes untracked files from the working directory.

## 5. Stashing

- **`git stash`**: Saves your local modifications temporarily and reverts your working directory to match the HEAD commit.
- **`git stash apply`**: Re-applies the changes saved in the stash.
- **`git stash pop`**: Applies the stash and then immediately removes it from the stash list.
- **`git stash list`**: Lists all stashes.

## 6. Tagging

- **`git tag [tag-name]`**: Creates a new tag for the current commit.
- **`git tag -a [tag-name] -m "[message]"`**: Creates an annotated tag with a message.
- **`git show [tag-name]`**: Displays information about a specific tag.
- **`git push [remote] [tag-name]`**: Pushes a specific tag to a remote repository.

## 7. Configuration

- **`git config --global user.name "[name]"`**: Sets the username for all repositories on your system.
- **`git config --global user.email "[email]"`**: Sets the email for all repositories on your system.
- **`git config --list`**: Lists all the Git configuration settings.

## 8. Git Aliases

- **`git config --global alias.[alias-name] '[git-command]'`**: Creates a custom alias for a Git command. For example, `git config --global alias.co checkout` will allow you to use `git co` instead of `git checkout`.

## 9. Advanced Commands

- **`git rebase [branch]`**: Re-applies commits from one branch on top of another base branch. Useful for keeping a clean commit history.
- **`git cherry-pick [commit]`**: Applies the changes from a specific commit onto the current branch.
- **`git bisect`**: Uses binary search to find the commit that introduced a bug.
- **`git reflog`**: Shows a log of changes to the local repository's reference history, including actions like commits, resets, and checkouts.

## 10. Collaboration Commands

- **`git blame [file]`**: Shows what revision and author last modified each line of a file.
- **`git shortlog`**: Summarizes `git log` output in a more human-readable format.
- **`git describe [commit]`**: Finds the most recent tag reachable from a commit.

## 11. Submodules

- **`git submodule add [repository-url] [path]`**: Adds a submodule to the repository.
- **`git submodule update --init --recursive`**: Clones and initializes all submodules.
- **`git submodule foreach [command]`**: Runs a command in each submodule.

## 12. Git Hooks

- **`git hooks`**: A directory that contains scripts which are executed at certain points in the Git workflow (e.g., pre-commit, post-commit).

## 13. Git Archive

- **`git archive [branch] --format=[zip|tar] --output=[filename]`**: Creates an archive of the specified branch in a specified format (zip or tar).

---

Feel free to explore these commands to improve your Git workflow!
