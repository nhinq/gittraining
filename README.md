# Git Push / Pull
//
cd your web/root

$ git clone git@github.com:nhinq/gittraining.git

$ git add .

$ git commit -m "your issue"

$ git push origin master

// or $ git push origin {BRANCH}

// of $ git push

//Pull code

$ git pull origin master

// or

$ git pull


# Git resovled conflict
Example we has 3 branch
$ master, stage, develop
//always start with master as your base branch

$ git checkout master

$ git pull origin master

$ git checkout -b NEW-BRANCH-CHANGE

//changes 

$ git push origin NEW-BRANCH-CHANGE

# PR to develop

//if conflict then do
# Solution 1

$ git fetch origin

$ git checkout -b NEW-BRANCH-CHANGE origin/NEW-BRANCH-CHANGE

$ git merge develop

//review & manual merge

$ git commit -m "NEW-BRANCH-CHANGE merged"

$ git push origin NEW-BRANCH-CHANGE

# Solution 2
$ git fetch origin

$ git checkout develop

$ git pull origin develop

$ git checkout -b NEW-BRANCH-CHANGE-Dev

$ git pull origin NEW-BRANCH-CHANGE

//review & manual merge

$ git commit -m "NEW-BRANCH-CHANGE-Dev merged"

$ git push origin NEW-BRANCH-CHANGE-Dev

//repeat for Stage and Master
