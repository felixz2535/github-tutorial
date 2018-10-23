# GitHub Tutorial

_by Felix_

---
## Git vs. GitHub

**Git** is a control version system.
That just mean that you can view changes, make changes, and go back on your changes.
This is very useful when you want to explore your works and projects. 

**Github** is server online that act as a remote for whatever you push from your local.
That means github is a place where you put your project.
As long as you have internet you can go to github and look at the project.

---
## Initial Setup
 #### Create a GitHub Account  
 To create your github account you'll have too first got to [github.com](github.com),
 following that click on _Sign Up_.
 #### Login to the GitHub Account
  After you've sign up you will need to sign in by clicking on the Sign In.
 #### Link the Account to your IDE with SSH key
 Depending on your IDE the way that you get your SSH key may vary but more or less the same.
 After you get your SSH key you'll have to enter it on github.
 On github go setting located on the top-right icon.
 On the sidebar, click on SSH and GPG.
 The click on the New SSH Key.
 Type in the wanted Title and the SSH given by your IDE and now you are set.

---
## Repository Setup
1. Go to github, login in
2. Click on the plus icon and select new repository
3. Enter name and click on Creat Repository
4. Copy the SSH from your repository
5. Go to the desinated location and create a directory
6. `git init` to create repository
7. Type in `git remote add origin SSH`
8. You are all set, you can do whatever you like like creating a file and the add > commit > push  



---
## Workflow & Commands
These are the most command command perform on git.
By knowing these basic you can explore git as you wish.

**`git init`**  
The command initializes your directory which should be one of your very first step when using git.
It lets git know what directory you want it to work on.  

**`git add`**  
The command adds your files to the stage this is so that you tell git that you are ready to commit the file(s)  

**`git commit`**  
The command takes a "screenshot" of your repository. This is kept so that you can track what changes you have made.
It is often acompanied by a message.  

**`git clone`**  
The command clones or makes a copy in your directory of the copyied files (forked or cloned)

**`git push`**  
After you hand commited you now need to push it.
By using this command you are sending the commit to the remote so that it can be accessed online or by other devices.  

**`git pull`**  
The command pulls the commit from a remote.
If you already have a bridge connected between your local and remote you can pull changes that was made by someone else or other devices.

**`git remote -u origin master`**  
The command creates a bridge between the remote and the local. This way you can simply do `git pull` and `git push` withou the extra `origin master` part that usally follows the command.   

**`git status`**  
This command is rated to be the most helpful command. Not only it can see your current stage but also suggest what you might want tot do next  

**`git remote -v`**  
To check the status of linked remote you can simply use this command. 

**`git diff`**  
If you ever wanted to compare the differences of your commits this command does the job.
It check what changes was made between two commits

**`git log`**  
This commits review preview commits along with the SHA which can be useful when you want to refer to it in other commands.  

**`q`**  
When you are in `git log` you might be confused as to what to do most of the time by pressing q you can exit the log  

**`rm -rf .git`**  
This command removes your .git if you ever accidentally initialized a directory or decides to destory the bridge between the local and remote. 

---
## Rolling Back Changes
Ever made a mistake in Editing, Adding, Commiting, or Pushing?
Of course you had this list of command is every help when it comes to rolling back changes.
You must be very thought proceding these command because when you roll back changes you are abandoning your current position.

**`git checkout -- file`**  
After you edited your file you may perfer the previous version over your current changes,
this is where this command come to use. It **"unedit"** you current file.   

**`git reset HEAD file`**  
When you add a file onto the stage you might want to **"unadd"** to do so you used this command, 
you could see this command recommanded by `git status` after you had added your file(s) to the stage. 

**`git reset --soft HEAD file`**  
If you every want to roll back on your commit you would want to use this command. It **"uncommit"** your previous commit.  

**`git reset HEAD~1`**   
After noticing you dont like you commit you previously made you can use this command to backtrace to the editing stage.
The function of this command is to simply **"uncommit" and "unadd"**  

**`git reset --hard HEAD file`**  
Lastly we have a command that does all of the following. It allows you to **"uncommit", "unadd", and "unedit"**

**`git reset --hard [first nine digit of SHA]`**  
This command deletes the commit you made from your remote.
You can thing it as **"Unpushing"** a file.