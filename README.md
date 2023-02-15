# Git Sheet Cheat

- Create a repository
    - git init /path/to/directory
- Set global variables
    - git config --global user.name "your name" 
    - git config --global user.email "your e-mail" 
    - `If you want to configurate the variables locally just remove the --global`
- See all variables
    - git config --list
- Add a file to the project
    - git add file-name
    - git add . 
    - `To add all files just put '.'`
- See all files in the staging area (not committed yet)
    - git status
    - git status `-v` 
        - Get more information, including the changes
    - git status `-s`
        - Less information it is showned
    - `man git-status`
        - Documentation fo the command git status
    - `git only shows the foulders that it is not empty, to add the foulder it is required to add a file or add a file .keep`
- Remove a file in the staging are
    - git rm file-name
- Commit files
    - git commit
    - git commit `-m` "message"
        - Commit the files in the staging area with a messge


## Functionalities

- .gitignore
    - List of ignored files, will not be tracked in the git 