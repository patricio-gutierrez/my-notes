# Git & Github

> Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## Why git is important?

- It lets you and your team work on a single project without conflicting with each other.
- It can give a timeline of your work so you can go back and compare with past work.

## .gitkeep

- Stages an empty folder to git.

## Commands

| Command                                                | What it does                                               |
| ------------------------------------------------------ | ---------------------------------------------------------- |
| `git --help`                                           | Shows man page for git.                                    |
| `git config --global user.name`                        | Configures global username for git.                        |
| `git config --global user.email`                       | Configures global user email for git.                      |
| `git config --global -e`                               | Edit global git config.                                    |
| `git config --global init.defaultBranch main`          | Changes global main branch name.                           |
| `git status`                                           | Displays information about the status of the files in git. |
| `git add <filename>`                                   | Add the file to git.                                       |
| `git add .`                                            | Adds all the untracked files to git.                       |
| `git reset <filename>`                                 | Remove file from git.                                      |
| `git commit -m "<message>"`                            | Commits the files to git with a message.                   |
| `git checkout -- .`                                    | Reverts changes in file to the last commit.                |
| `git branch`                                           | Display in which branch your are currently working.        |
| `git commit -am "<message>"`                           | Commits only tracked files to git with a message.          |
| `git log`                                              | Show commit logs of all files.                             |
| `git config --global alias.<alias_name> <git_command>` | Creates alias for git command.                             |
