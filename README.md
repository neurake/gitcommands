# gitcommands
git commands

git add filename.ext - To add a particular file in the staging area.
git add - To add all files in the staging area.
git restore --staged filename.ext - To unstage a particular file.
git diff - compare the working directory with the staging area.
git commit -m "any message" - Commit into a final folder with the message.
git commit -a -m "any message" - Commit into a final folder skipping staging area with the message.
git commit --amend - To change the commit.
git diff --staged - Compare the staging area to the last commit.
git checkout --filename.ext - Change a particular file data to the last commit.
git checkout -f - Change all file data to the last commit.
git log - To see all commits.
git log -p - To see the information about what was deleted and added in all commits.
 git log -p - n - To see the information about what was deleted and added in 'n' commits.
 touch filename.ext - To create a new file.
git mv filename.ext renamed name.ext - rename a particular file and move the file to the staging area.
git rm filename.ext - to delete a particular file and move the file to the staging area.
git rm --cached filename.ext - to stop tracking a particular file.
git checkout -b new branchname - to create a new branch and move to that new branch.
git checkout branchname - to move to a particular branch.
git branch - to see all branches and current branch in pwd.
git merge branchname - to merge into a master branch if merge conflicts happen you have to fix it manually and then stage the file by running `git add .` command and then commit by running `git commit -m "any message"`.
 git branch -v - to see the last commits of all branches.
 git branch --merged - to see merged branches.
git branch --no-merged - to see non-merged branches.
 git branch -d branchname - to delete a non-merged particular branch but it will not delete rather it will give a warning that your branch is not merged. After the warning, you want to delete replace small d with capital d and your branch will be deleted.
git branch -D branchname - to delete a particular branch.
rm -rf .git - to stop tracking the folder or you can say that make a non-git folder.
Now, we will move to see how we can easily use Github using Git commands - 

First, create an account on Github. Make a repository and then add ssh keys to GitHub. To generate an ssh key follow the commands:

ssh-keygen-t rsa -b 4096 -C "your email"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
tail ~/.ssh/id_rsa.pub    
How to push files and folders in the GitHub repository?

git remote: To check if any remote account is connected or not.
git remote -v: To check from where we can push our files or from where we can pull the files.
git remote add origin "url of github repository": To add GitHub repository to git/local storage.
git push -u origin master - to push files into GitHub repository.
git push origin branchname: To push a particular branch into GitHub repository.
git push origin branchname::newbranchname: To push a particular branch into GitHub repository as a new name.
git push -d origin branchname: To delete a branch in the GitHub repository.
How can you clone anyone GitHub repository in your local system?

git clone "url" - to clone GitHub repository in local storage as the default name.
git clone "url" new name - to clone GitHub repository in local storage as a new name.




Categories are as follows:

To create
To make local changes
To commit history
Branches and tags
To update and publish
To merge and reuse
To undo
Let us do define commands that do fall under these categories that are listed below as follows:  

Type 1: CREATE

Clone an existing repository: git clone
Create a new local repository: git init
Type 2: LOCAL CHANGES

Changed files in your working directory: git status
Changes to tracked files: git diff
Add all current changes to the next commit: git add
Add some changes to the next commit: git add -p
Commit all local changes In tracked files: git commit -a
Commit previously staged changes: git commit
Change the last commit: git commit --amend
Type 3: COMMIT HISTORY

Show all commits. starting with newest: git log
Show changes over time for a specific file: git log -p
Who changed what and when in: git blame
Type 4: BRANCHES & TAGS

List all existing branches: git branch -av
Switch HEAD branch: git checkout
Create a new branch based on your current HEAD: git branch
Create a new tracking branch based on a remote branch: git checkout - -track
Delete a local branch: git branch -d
Mark the current commit with a tag: git tag
Type 5: UPDATE and PUBLISH

List all currently configured remotes: git remote -v
Show Information about a remote: git remote show
Add new remote repository, named remote: git remote add
Download all changes from but don't integrate into HEAD: git fetch
Download changes and directly merge/integrate into HEAD: git pull
Publish local changes on a remote: git push
Delete a branch on the remote: git branch -dr
Publish your tags: git push --tags
Type 6: MERGE & REUSE

Merge into your current HEAD: git merge
Rebase your current HEAD onto git rebase
Abort a rebase: git rebase - -abort
Continue a rebase after resolving conflicts: git rebase - -continue
Use your configured merge tool to solve conflicts: git mergetool
Use your editor to manually solve conflicts and (after resolving) mark tile as resolved: git add, git rm
Type 7: UNDO

Discard all local changes in your working directory: git reset -hard HEAD
Discard local changes in a specific file: git checkout HEAD
Revert a commit (by producing a new commit with contrary changes): git revert
Reset your HEAD pointer to a previous commit and discard all changes since then: git reset --hard
Preserve all changes as unstaged changes: git reset
Preserve uncommitted local changes: git reset - - keep





List of Top Useful Git Commands
Git commands are crucial for efficient collaboration and project management. In this article, we'll explore a list of important Git commands like git commands to push, git commit command, git pull command, and git push command, etc that will help to improve workflow and optimize productivity. These are a Git Commands list that can be used frequently on Git.

1. git help
Take help from the Git help section for different commands and other errors.  

git help       //Get help on Git Commands
2. git config
To set the basic configurations on Git like your name and email.

git config       // Set config values

  3. git config –-global user.name “ ”
Sets configuration values for your user name on git. 

git config –-global user.name “Ashish Madaan”    //Set global username


4. git config –-global user.email " "
Sets configuration values for your user email on git.  

git config –-global user.email ashishmadaan6@gmail.com     // Set global email


5. git config –-global color.ui
To see different colors on the command line for different outputs.  

git config –-global color.ui true                           //  Enable color highlighting       


6. mkdir
Create a directory if not created initially. 

mkdir store                                                     // Create a new directory


7. cd
To go inside the directory and work on its contents.  

cd store                                                  // Enter directory        


8. git init
To create a local git repository for us in our store folder. This will help to manage the git commands for that particular repository.  

git init                                                 // Initialize Git repo


9. git status
To see what's changed since the last commit. It shows all the files that have been added and modified and are ready to be committed and files that are untracked.  

git status                                            //Check repo status


10. git add Readme.txt
To add a file Readme.txt to the staging area to track its changes.  

git add Readme.txt                          // Add Readme.txt file to the staging area


11. git commit -m “ ”
To commit our changes(taking a snapshot) and provide a message to remember for future reference.

git commit -m “Created a Readme.txt”        // Commit staged changes with a descriptive message


 12. git log
To check the history of commits for our reference. 

git log                                                  // View commit history with details like author, date, and message


13. git add
To add a specific list of files to the staging area.  

git add                                             // Add specific files to the staging area (must specify filenames)


14. git add --all
To add all files of the current directory to the staging area. 

git add --all                                 // Stage all files (tracked and untracked) in the current directory


15. git add *.txt
To add all text files of the current directory to the staging area.

git add *.txt                              // Stage all .txt files in the current directory 


  16. git add docs/*.txt
To add all text files of a particular directory(docs) to the staging area. 

git add docs/*.txt                     // Stage all .txt files inside the 'docs' folder


17. git add docs/
To add all files in a particular directory(docs) to the staging area.

git add docs/                          // Stage all files inside the 'docs' directory


 18. git add “*.txt”
To add text files of the entire project to the staging area. 

git add “*.txt”                         // Stage all .txt files across the entire project (quotes handle globbing) 


19. git diff
To figure out what changes you made since the last commit.

git diff                                 // Show file changes not yet staged for commit


 20. git reset head license
To undo the staging of the file that was added in the staging area.

git reset head license         // Unstage the 'license' file that was previously added


21. git checkout –license
To Blow away all changes since the last commit of the file.

git checkout –license             // Discard local changes to 'license' file (revert to last commit)


22. git commit -a -m “ ”
To add any of our tracked files to the staging area and commit them by providing a message to remember.

git commit -a -m “Readme.md”     //Automatically stage tracked files and commit with a message


23. git reset –soft HEAD^
To undo the last commit and bring the file to the staging area.

git reset –soft HEAD^                  // Undo last commit, keep changes in staging area



 24. git reset –hard HEAD^
To undo the last commit and remove the file from the staging area as well(In case we went horribly wrong).

git reset –hard HEAD^


25. git reset –hard HEAD^^
To undo the last 2 commits and all changes.

git reset –hard HEAD^^


26. git remote add origin
These commands make a bookmark which signifies that this particular remote refers to this URL. This remote will be used to pull any content from the directory and push our local content to the global server.

git remote add origin https://github.com/madaan123/MyAlgorithms


27. git remote add <address>  
To add new remotes to our local repository for a particular git address.

git remote add <address> 


 28. git remove rm
To remove a remote from our local repository.

git remove rm


29. git push -u origin master
To push all the contents of our local repository that belong to the master branch to the server(Global repository).

git push -u origin master


30. git clone https://github.com/madaan123/MyAlgorithms
To clone or make a local copy of the global repository in your system 
(git clone command downloads the repository and creates a remote named origin which can be checked by the command – git remote -v). 

git clone https://github.com/madaan123/MyAlgorithms


31. git branch Testing
To create a new branch named Testing.

git branch Testing


32. git branch
To see all the branches present and current branches that we are working on.

git branch


33. git checkout Testing
To switch to branch Testing from the master branch. 

git checkout Testing


34. ls
To see directories and files in the current directory.  

ls


35. ls -la
To see hidden directories and files within the current directory.

ls -la


36. git merge Testing
To merge the Testing branch with the master branch.  

git merge Testing


37. git branch -d Testing
To delete the Testing branch.  

git branch -d Testing


38. git checkout -b admin
To create a new branch admin and set it as the current branch.

git checkout -b admin


39. git branch -r
To look at all the remote branches.

git branch -r


40. git branch -D Testing 
To forcefully delete a branch without making commits.  

git branch -D Testing


41. git tag
To see the list of available tags. 

git tag


42. git checkout v0.0.1
To set the current tag to v0.0.1. 

git checkout v0.0.1


43. git tag -a v0.0.3 -m “version 0.0.3”
To create a new tag. 

git tag -a v0.0.3 -m “version 0.0.3”


44. git push –tags
To push the tags to the remote repository.

git push –tags


45. git fetch
To fetch down any changes from the global repository to the current repository.

git fetch


46. git stash
To move staged files to the stash area which is present in the staging area.

git stash 


47. git stash pop
To get back the files that are present in the stash area.

git stash pop


48. git stash clear
To clear the stash folder.

git stash clear


49. git rebase
Three tasks are performed by git rebase 

Move all changes to master which are not in origin/master to a temporary area.
Run all origin master commits.
Run all commits in the temporary area on top of our master one at a time, so it avoids merge commits.
git rebase


50. git –version
used to show the current version of Git

git –version
