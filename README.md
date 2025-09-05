# gitcommands
git commands


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
