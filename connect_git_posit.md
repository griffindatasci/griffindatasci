# Short notes on Git, GitHub and RStudio/Posit

These are the notes I took while reading and working through the excellent guide [Let's Git Started](https://happygitwithr.com/index.html). I made these notes as a quick reference to myself, but they should be detailed enough that &mdash; with luck &mdash; they are useful to others (so i've put them in a public repo). I very much recommend reading the Let's Git Started guide too and checking there if you encounter any issues!

### Prerequisites

1. Install RStudio/Posit (herein, Posit)
1. Install Git
1. Create a GitHub account

### Connecting and Testing Git & GitHub

1. Open Posit, and in the terminal, execute:
  - `git config --global user.email '<email@address.here>'` in the terminal to set your user email
  - `git config --global user.name '<username here>'` in the terminal to set your user name
  - `git config --global init.defaultBranch main` in the terminal to set default initial branch to main (not master)
1. Open GitHub in your browser and create a repository (repo)
1. Click the green code button and copy the https url
1. In the Posit terminal, use `cd` to navigate to the directory that will contain the GitHub repo on your local machine (use `cd ..` to navigate up a directory and `ls` to see contents of a directory)
1. In the Posit terminal, clone the repo using `git clone <url>`
1. In the Posit terminal, `cd` into that repo
1. Modify the *README.md* file and save it
1. In the Posit terminal, execute:
  - `git add` to stage the change(s)
  - `git commit -m <a useful commit message>` to commit the change(s)
  - `git push` to push the changes to GitHub
1. In your browser, check the changes are present in the README.md file on your GitHub account

If this did not work, head to [Let's Git Started](https://happygitwithr.com/index.html) &mdash; the much more in depth guide that I based these notes on &mdash; to get more detailed instructions and troubleshooting help. Check out the *Can you hear me now?* section.

### Using GitHub and Posit

The best approach is to create the repo on GitHub, then connect it to a project in Posit.

##### Initiating a new repo and project 

1. Create a new repo on GitHub and copy the url
1. In Posit, go to *file* > *new project* > *version control* > *git*
1. Paste in the repo url, choose location for the repo on the local machine, check *open in new session*, click *create project*


##### Stage, commit and push from Posit


Once you have created a project, it can contain scripts, data, outputs etc. that you will create and modify. Changes can then be uploaded to GitHub by staging, committing and pushing these changes.

1. Make and save changes to your files
1. In Posit, go to the *Git* tab
1. Check staged on file(s) to be uploaded
1. Click *commit*
1. Add a useful commit message
1. Click *commit*
1. Close the *Git Commmit* message box
1. Click *push*
1. Close the *Git Push* message box

*Check the GitHub repo online to make sure the push worked!*


### Useful bash commands

- `cd` - change directory
- `rm -rf <path>/` - remove a directory/repo
- `git status` - shows if files are modified
- `git add <file.ext>` - to stage
- `git commit -m "<message>"` - to commit
- `git push` - to push
- `git config --global --list` - to see current git credentials
- `git config --global --edit` - to edit current credentials
- `git config --global --unset <credential> ` - to remove a credential
- `git config --global init.defaultBranch main` - to set default branch to main
