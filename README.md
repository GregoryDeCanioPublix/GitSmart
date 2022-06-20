<a name="BackToTop"></a>

# GitSmart

## Table of Contents
- [Git_Speedrun](#Git_Speedrun)
- [Git_Commands_In_Detail](#Git_Commands_In_Detail)
- [Setting_Up_GitHub_for_the_First_Time?](#Setting_Up_GitHub_for_the_First_Time?)
- [Favorite_Git_Resources](#Favorite_Git_Resources)

Unless stated otherwise, assume you are running all commands in Windows PowerShell.

---

<a name="Git_Speedrun"></a>  

## Git_Speedrun  
Set-Location C:\Users\P1603119\Desktop\GitHub\GitSmart  
git remote update  
git status  
*Pull is only needed if your branch is behind origin/main*   
git pull origin main  
git add - A  
git commit -a -m "COMMENT"  
git push origin main  

---

<a name="Git_Commands_In_Detail"></a>  

## Git_Commands_In_Detail  
**To work on an up-to-date copy of the project, pull to get all the changes made by users**   
*(When you clone a repository, REMOTE is typically the origin)*    
git pull *REMOTE* *name-of-branch*  
git pull origin main  

**Create a new branch**  
git checkout -b *name-of-branch*

**Create a new branch on a different existing branch**  
*(Best practice to Pull Origin beforehand to ensure you are working with the most recent version)*   
git branch *new-branch* *base-branch* 

**Switch to a branch**    
git checkout *name-of-branch*    

**Publish local branch to your remote repository:**    
git push -u origin *local-branch*   

**Update all of your branches (that are set to track remote ones). This does not update or make any actual changes**  
git remote update   

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

**To list all branches in local and remote repositories**   
git branch -a

**To list only branches in the remote repository**   
git branch -r

---

<a name="Setting_Up_GitHub_for_the_First_Time?"></a>

## Setting_Up_GitHub_for_the_First_Time? 
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

<a name="Favorite_Git_Resources"></a>

---

## Favorite_Git_Resources   
https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html

[Back to Top](#BackToTop)