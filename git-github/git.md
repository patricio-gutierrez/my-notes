# Git & Github

> Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Why git is important?

- It lets you and your team work on a single project without conflicting with each other.
- It can give a timeline of your work so you can go back and compare with past work.

## .gitkeep

- Stages an empty folder to git.

## .gitignore

- Ignores specified files or folders.

## Git Commands

| Command                                                | What it does                                                                                                                                                               |
| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git --help`                                           | Shows man page for git.                                                                                                                                                    |
| `git config --global user.name`                        | Configures global username for git.                                                                                                                                        |
| `git config --global user.email`                       | Configures global user email for git.                                                                                                                                      |
| `git config --global -e`                               | Edit global git config.                                                                                                                                                    |
| `git config --global init.defaultBranch main`          | Changes global main branch name.                                                                                                                                           |
| `git status`                                           | Displays information about the status of the files in git.                                                                                                                 |
| `git add <filename>`                                   | Add the file to git.                                                                                                                                                       |
| `git add .`                                            | Adds all the untracked files to git.                                                                                                                                       |
| `git reset <filename>`                                 | Remove file from git.                                                                                                                                                      |
| `git commit -m "<message>"`                            | Commits the files to git with a message.                                                                                                                                   |
| `git checkout -- .`                                    | Reverts changes in file to the last commit.                                                                                                                                |
| `git branch`                                           | Display in which branch your are currently working.                                                                                                                        |
| `git commit -am "<message>"`                           | Commits only tracked files to git with a message.                                                                                                                          |
| `git log`                                              | Show commit logs of all files.                                                                                                                                             |
| `git config --global alias.<alias_name> <git_command>` | Creates alias for git command.                                                                                                                                             |
| `git diff`                                             | Shows the changes since the last commit.                                                                                                                                   |
| `git diff --staged`                                    | Shows the changes only in stage since the last commit.                                                                                                                     |
| `git commit --amend -m "<message>"`                    | Edits the last commit message.                                                                                                                                             |
| `git reset --soft HEAD^<number>`                       | Deletes last commit or if number specified the number of that commit.                                                                                                      |
| `git reset --mixed HEAD^<number>`                      | Deletes last commit or if number specified the number of that commit and keeps changes.                                                                                    |
| `git reset --hard HEAD^<number>`                       | Deletes last commit or if number specified the number of that commit and reverts changes.                                                                                  |
| `git reflog`                                           | Shows timeline of everything thats happend in the repository.                                                                                                              |
| `git branch <name>`                                    | Creates branch with name.                                                                                                                                                  |
| `git checkout <name>`                                  | Changes to name branch.                                                                                                                                                    |
| `git merge <name>`                                     | Merges the specified branch to the actual branch.                                                                                                                          |
| `git branch -d <name> -f`                              | Deletes the specified branch.                                                                                                                                              |
| `git checkout -b <name>`                               | Creates a branch and moves to that branch.                                                                                                                                 |
| `git tag <name>`                                       | Adds tag to commit.                                                                                                                                                        |
| `git tag -d <name>`                                    | Deletes tag.                                                                                                                                                               |
| `git tag -a <name> -m "<message>"`                     | Adds tag with description.                                                                                                                                                 |
| `git show <tag>`                                       | Shows all information about that tag.                                                                                                                                      |
| `git stash`                                            | Temporarily stores (or stashes) the changes you've made to the code you're working on so you can work on something else, and then come back and reapply the changes later. |
| `git stash list`                                       | Lists all the current stashes.                                                                                                                                             |
| `git stash pop`                                        | Merges the stash to the current branch.                                                                                                                                    |
| `git stash clear`                                      | Clears all the stashes.                                                                                                                                                    |
| `git stash apply <number>`                             | Merges the specific number stash.                                                                                                                                          |
| `git stash drop <number>`                              | Deletes the specified number stash.                                                                                                                                        |
| `git stash save "<message>"`                           | Saves stash with message.                                                                                                                                                  |
| `git rebase <branch>`                                  | Rebases is the process of moving or combining a sequence of commits into a new base commit.                                                                                |
| `git rebase -i <branch>`                               | Rebases is the process of moving or combining a sequence of commits into a new base commit.                                                                                |
| `git add remote origin <url>`                          | Add a remote git repository from the specified url.                                                                                                                        |
| `git push origin <branch>`                             | Pushes files and folders to remote git repository.                                                                                                                         |
| `git push --tags`                                      | Pushes tags to remote git repository.                                                                                                                                      |
| `git pull`                                             | Pulls changes made on the remote git repository.                                                                                                                           |
| `git config --global pull.ff only`                     | When pulling from a remote git repository, it only accepts it if its fast forward.                                                                                         |
| `git remote -v`                                        | Check to which remote git repository you are connected.                                                                                                                    |
| `git clone <url>`                                      | Clones files from remote git repository.                                                                                                                                   |
| `git config pull.rebase true`                          | Sets pull mode to rebase.                                                                                                                                                  |
| `git fetch`                                            | Fetches latest data from remote repository without doing pull request.                                                                                                     |
