## GITHUB CHEATSHEET

Pulling from master to local repository

  git init (only first time)
  git remote add upstream <master repository url> # (only first time)
  git pull upstream master <master repository url>

Pushing from local repository to personal fork. This is
however only necessary when you plan on doing a pull
request to the master

  git push origin master

Committing changes to the local repository:
  git commit -m <commit message>

### Creating a new repository
 - Go to your own github page @ https://github.com/<github username>
 - Click New repository
 - Define a <repository name>
 - Provide a description
 - Choose public (or private if you wish to pay the required fee of $7.00/month)
 - Choose wheter or not you wish to create the new repository with a README file
 - Click Create repository
 - Open your prefered terminal and execute the following
  git config --global user.name "Your name"
  git config --global user.email your@email.domain
  mkdir <repository name>
  cd <repository name>
  git init
  <place files to be versioned into current directory>
  git commit -m 'First addition of all files'
  git remote add origin git@github.com:<github username>/<repository name>.git
  git push -u origin master
      
### Pushing a new repository into github

  cd <existing repository name>
  git remote add origin git@github.com:<github username>/<repository name>.git
  git push -u origin master
  
### Creating a new branch and switching to it right away
  git checkout -b <new branchname> <branchname to branch from>

### Reverting a file to its last committed state
  git checkout -- <file>