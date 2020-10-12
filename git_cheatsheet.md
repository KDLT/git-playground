#### Terminal commands
`ls`lists all of the folders  
`ls -la` lists all of the files  
`cd ..`  returns one dir back   
`cd` enters a directory  
`.` - just install in the current directory  
	
#### Initial install
`git --version` checks the version of the installed locally git  
`git config --global user.name "Your Name"` sets up the name of the user   
`git config --global user.email "yourname@somemail.eu"` sets up the mail of the user  
`git config --list` lists all the git configurations  
	
#### Getting Help
`git help <verb>` (e.g. git help config) OR   
`git <verb> --help`   
	
#### Initializing a Project
`git init` initializes the git repo in the current folder  
`touch .gitignore` creates a git ignore file  
`git status` check working tree, both on the git and on local  
  
#### Adding files
`git add -A` adds all of the files for commiting  
`git add .` also works but only with respect to present working directory
	  
#### Removing files
`git reset` removes files to be commited   
`git reset uncommitme.js` removes uncommitme.js from the commit preparation  
	  
#### Committing
`git commit -m "This is the commit message"` -m is used to add message  
	  
#### Checking Log
`git log` renders commit ids, authors, dates  
	  
#### Cloning a Remote Repo
`git clone <url> <where to clone>`
  
#### View Repository Information
`git remote -v` lists infor about the repo  
`git branch -a` lists all of the branches  
  
#### View Changes
`git diff` shows the difference made in the files  
	  
#### Pulling from Master Branch on Origin
`git pull origin master` the word origin is specified in `./.git/config` can be another name of your choosing. For posterity, origin is used. **Keep a habit of pulling before pushing**
	  
#### THEN PUSH
`git push origin master` <origin> name of remote repo <master> the branch that we push to   
	  
#### First time push of the branch
`git push -u origin <name of the branch>` -u coordinates the two branches (local and on server)  
	  
#### Create a branch
`git branch <name of the branch>`  
  
#### Checkout a branch
`git checkout <name of the branch>`  
  
#### Merge a branch
`git checkout master`  
`git pull origin master`  
`git branch --merged` see which branches are merged   
`git merge <name of the branch you want to merge>`  
`git push origin master`  
  
#### Delete a branch
`git branch -d <name of the branch>` this deletes it locally!!!  
`git branch -r` list branches in remote only  
`git branch -a` list branches in both remote and local   
`git push origin --delete <name of the branch>` this deletes it from the repo!  
  
#### Reset branch to a previous HEAD
`git reflog --relative-date` list all the heads tagged with a relative time from now  
`git reset` --hard <commit id>` commit id is the first column of the result of reflog  
  
#### Branching Guideline
- `git push origin` markdown created a new branch and pull request on remote  
- `git push origin`  
