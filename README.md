# Git Sheet Cheat

Some informations about how to use git in the CLI.

## Commands

- ***Create a repository***
    - `git init <path-to-directory>`
- ***Set global variables***
    - `git config --global user.name "your name"` 
    - `git config --global user.email "your e-mail" `
    - If you want to configurate the variables locally just remove the --global
- ***See all variables***
    - `git config --list`
- ***Add a file to the project***
    - `git add <file-name>`
    - `git add . `
    - To add all files just put '.'
- ***See all files in the staging area (not committed yet)***
    - `git status`
    - `git status -v` 
        - Get more information, including the changes
    - `git status -s`
        - Less information it is showned
    - `man git-status`
        - Documentation fo the command git status
    - git only shows the foulders that it is not empty, to add the foulder it is required to add a file or add a file .keep
- ***Show the historic of the commits***
    - `git logs`
    - Example: `git log --oneline`
        - Show all the historics in one line.
    - `git log --stat`
        - Show the statistics of the files with each commit
    - `git log --graph`
        - Show the textual graph of the project`s commit
- ***Remove a file in the staging area***
    - `git rm <file-name>`
- ***Commit files***
    - `git commit`
    - `git commit -m "<message>"`
        - Commit the files in the staging area with a messge
- ***Create an annotated tag***
    - `git tag -a <tag-name> -m <message>`
    - Has full information about the branch
- ***View all tags in a repository***
    - `git tag`
- ***Create a lightweight tag***
    - `git tag <tag-name> -m <message>`
- ***Delete a tag***
    - `git tag -d <tag-name>`
- ***Create a new branch***
    - `git branch <branch-name>`
- ***Switch to another branch***
    - `git checkout <branch-name>`
- ***Delete a branch***
    - `git branch -d <branch-name>`
- ***Combine the lastest commits from two branch into one branch***
    - `git merge <branch-name>`
- ***Replay changes made to one branch over the top of another branch***
    - `git rebase <branch-name>`
- ***Revert a commit in the project***
    - `git revert <commit-name>`
    - Example: `git revert HEAD`
        - Revert the latest commit
- ***Show the difference in the files***
    - `git diff`
- ***Clone a repository***
    - `git clone <remote-repository-address>`
        - Clone a remote repository
    - `git clone <local-repository> <new-repository>`
        - Clone a local repository
- ***Show the remote servers that are being tracked for the current repository***
    - `git remote -v`
    - `git remote show origin`
        - show more details about the remote repository
- ***Fetch new commit informations***
    - `git fetch`
- ***Pushes local changes to the git repository***
    - `git push -u <remote-branch> <local-branch>`
    - `git push origin <local-branch>:<remote-branch>`
---

## Functionalities
- ***.gitignore***
    - List of ignored files, will not be tracked in the git.
- ***HEAD***
    - Point to the current branch.
- ***Forking a git project***
    - Basecally clone a project in another server, allowing others to work in another repository.
---

## SSH Key
1) Generate SSH key
    - `ssh-keygen -t ed25519 -C "your_email@example.com"`
2) Turn on the ssh-agent
    - `eval "$(ssh-agent -s)"`
3) Add your new SSH key in the ssh-agent
    - `ssh-add ~/.ssh/id_ed25519` or the path of your private key
4) Copy your ssh key
    - `clip < ~/.ssh/id_ed25519.pub` or the path of your bublic key
5) Paste your key in the SSH and GPG keys in the GitHub

---
### Credits

 - Information get by studing in the website [A CLOUD GURU](https://learn.acloud.guru/).

