# 2023-01-17: DSCI 310 git demo
Intro git demo review

- `git clone <URL>` : takes what's on github and does a one time download to your computer
- `git status` : tells you what's going on in the repository
- `git add <FILE>` : add the <FILE>s to the staging area
- `git commit`: create the commit (aka snapshot)
    - `git commmit -m "MESSAGE"` : create the git message directly in the command line

- `git push <where> <what>` : take local commits on `what`,  and send it to `<where>`
    -e.g. , `git push origin main`
    - `git push origin main`: sends code from branch `main` local computer to the remote `origin`
- `git pull <where> <what>` : take remote commits on `what`,  and pull from `<where>`
    - e.g. , `git pull origin main`

- `git log --oneline --graph --all` : shows you all your history


## Branches

- `git branch <name>` : create a branch named <branch> where ever you are (`HEAD`)
- `git switch <name>` : go to that branch 
    - `git  checkout <name>` : older way to move to branch
- `git switch -c <name>` : create a branch and move to it in 1 command
    - `git checkout -b <name>` : same thing using `checkout`


## Cleanup process

1. delete branch PR in github
2. `git fetch --prune` : update references to deleted branches on the remote
3. `git branch -d <name>` : delete local branch `<name>`
