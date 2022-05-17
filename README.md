# GitSmart

Unless stated otherwise, assume you are running all commands in Windows PowerShell.


## Routine Git Commands  
**Download the latest changes in the project**  
git pull *REMOTE* *name-of-branch*

**Create a new branch**  
git checkout -b *name-of-branch*

**Create a new branch on a different existing branch**  
*(Best practice to Pull Origin beforehand to ensure you are working with the most recent version)*   
git branch *new-branch* *base-branch* 

**Switch to a branch**    
git checkout *name-of-branch*    

**Publish local branch to your remote repository:**    
git push -u origin *local-branch*   

**To check which files have been changed:**    
git status  

**To stage all (new, modified, deleted) files**   
git add - A

**To stage a file for commit:**   
git commit *file-name OR folder-name*

**To stage all files for commit:**   
git commit -a -m "COMMENT TO DESCRIBE THE INTENTION OF THE COMMIT"

**Send changes to GitHub:**   
git push *remote* *name-of-branch*

**To Push to main:**   
git push origin main

**To work on an up-to-date copy of the project, pull to get all the changes made by users**   
*(When you clone a repository, REMOTE is typically the origin)*    
git pull *REMOTE* *name-of-branch*    
git pull origin main   

**To list all branches in local and remote repositories**   
git branch -a

**To list only branches in the remote repository**   
git branch -r


## Setting up GitHub for the first time? 
First, make sure you set up a GitHub account and also downloaded Git to your computer    
*Do not use your personal GItHub account. Make a new one!*    

**To access the proxy reading the help file**   
git config –list   

**To link your GitHub account**     
git config --global user.name "your_username"   
git config --global user.email "your_email_address@example.com"

** You also need to access GitHub.com via a proxy. Note, this may not work in 2023 onwards***    
git config --global --replace-all http.proxy http:\domain.local\**PublixUsername*:*ComputerPassword*@webproxy1.publix.inet:9090

**Now that you machine is configured, follow these steps:**    
1. Change directory to where you want to maintain GitHub files      
For example: Set-Location *C:\Users\P1603119\Desktop\GitHub*   

2. Clone to that directory   
Example code:   
git clone https://github.com/GrossProfitSmart/GitSmart.git   
*(This will create a new folder in that directory which is where your git repository lives)*

3. Change directory again so you can start working in that repo!   
Example code:   
Set-Location *C:\Users\P1603119\Desktop\GitHub\GitSmart*


## Favorite Git Resources:   
https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html