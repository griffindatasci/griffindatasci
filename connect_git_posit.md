# How to connect Git, GitHub and RStudio/Posit

### Prerequisites

1. Install RStudio/Posit (herein, Posit)
2. Install Git
3. Create a GitHub account

# Connecting and Testing Git & GitHub

1. Open Posit
2. In the Posit terminal, execute:
  - `git config --global user.email '<email@address.here>'` in the terminal to set your user email
  - `git config --global user.name '<username here>'` in the terminal to set your user name
  - `git config --global init.defaultBranch main` in the terminal to set default initial branch to main (not master)
3. Open GitHub in your browser and create a repository (repo)
4. Click the green <code> button and copy the https url
5. In the Posit terminal, use `cd` to navigate to the directory that will contain the GitHub repo on your local machine (use `cd ..` to navigate up a directory and `ls` to see contents of a directory)
6. In the Posit terminal, clone the repo using `git clone <url>`
7. In the Posit terminal, `cd` into that repo
8. Modify the *README.md* file and save it
9. In the Posit terminal, execute:
  - `git add` to stage the change(s)
  - `git commit -m <a useful commit message>` to commit the change(s)
  - `git push` to push the changes to GitHub
10. In your browser, check the changes are present in the README.md file on your GitHub account


# New git/rstudio project

1. new repo
1. get clone repo https url
1. in posit, *file* > *new project* > *version control* > *git*
1. paste repo url, choose location for save on local machine, check *open in new session*, click *create project*


# stage, commit and push from posit

1. make and save changes
1. go to git tab
1. check staged on file(s)
1. click *commit*
1. add commit message
1. click commit
1. close the Git Commmit message box
1. click push
1. close the Git Push message box





# Useful bash commands
`git status` - shows if files are modified
`git add <file.ext>` - to stage
`git commit -m "<message>"` - to commit
`git push` - to push
`cd` - change directory
`rm -rf <path>/` - remove a directory/repo

To see, edit or remove current credentials respectively:

```
git config --global --list
git config --global --edit <credential>
git config --global --unset <credential>
```
git config --global init.defaultBranch main
