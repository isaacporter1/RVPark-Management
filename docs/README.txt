This was a Mock RV Park Management System for a local RV Park

git commands 

- git clone https://github.com/CS3750-Team3/RVPark.git - If you do not have any type or branch of the remote repo "RVPark" on your computer, use this command

- git branch - shows all the current local branches
- git branch yourname/branchName - creates a branch
- git branch -d yourname/branchName - deletes a local branch

These are the default commands for uploading your branch to the remote repository
- git checkout -b yourname/branchName - this will create a branch (if not already created) and switch to it on your local repo. Setting it up to be committed.
- git add . or filename - this will add whatever file or all files into a "commit" to then be able to push it to the remote repo
- git commit -m "Message" - This will commit your changes with a message
- git push -u origin yourname/branchName - this will push the new branch to the remote repo, and create an upstream link between them

If someone updated the master branch, and you dont have any changes you want to update, look below:
- git fetch origin - this will fetch the latest changes of the master branch to update your local repo WITHOUT merging them (meaning it will basically wipe your current local repo with the master branch repo)
- git checkout master - this will switch from whatever branch you were on to the master branch
- git pull origin master - this will pull all of the changes from the master branch into your local repo
- git checkout -b yourname/branchName - this will again switch your current local repo to be apart of a different branch that is not the master branch. So when updating the remote repo, it does not affect the master branch.

If someone updated the master branch, AND YOU DO HAVE CHANGES THAT YOU NEVER COMMITTED AND PUSHED, look below:
- git switch master - this will switch your local branch to the local master branch (what your computer thinks is the remote master branch)
- git fetch origin - this will fetch the new changes made to the master branch, comparing it to your old master branch that you first pulled from
- git pull origin master
- git checkout <your_branch_name>
- git merge origin/master or origin/branchname - this will attempt to merge your old local master branch or personal branch, with the new remote master branch (one on github)
  Once that is done, now you can merge your personal branch with the "new" master branch
- You will then have to update your branch immediately I believe, using the Visual Studio "Source Control" stuff, I could not find a way to do it through the terminal

Isaac's (me) directory was being wack, so I had to use this: git config --global --add safe.directory 'C:/Users/iporter/Documents/School - Weber/CS 3750/RVPark'
to give myself permissions
okay

COOL!
