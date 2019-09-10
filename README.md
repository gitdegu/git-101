# git-101

# Introduction
This is a resource mainly targeting to provide over all and general aspects of the git. The topic covers downlaoding, installtion, 
and working environment of git, and its related commands that could let the user to work with a version management operation.

# What is Git? 
-	It is a platform that could let a certain resource to be distributee across different people takig their won versions.

# What is version control? 
-	It is refering the different content that a certain shared resource has over the course time. such version control is  useful to work in teamand release the different version of the shared resource whenever a new version merges to the old one.


# Installtion of git
git can be downlaoded from the efollowing link  as per the kind of operating system you have
https://git-scm.com/downloads

# Already installed git 
The following link will provide the latest developmen verison for the git itself. Run the following command on the terminal
git clone https://github.com/git/git. It willautomatically update the git.

# Checking the version of git
git --version
it will show you the installed version of the git. Example : - git version 2.22.0

# Begin using the git
In order to begin using the git, the first thing that we shoudl do is  creating a folder using the command mkdir <folderName>
	Example : - mkdir git-102
	
Running the git
In order to initilize and run the git, oepn the folder you jsut created, and type on the terminal the following command
-	cd <folderName>
-	git init
	*	it will create an empty Git repository locally. The following message is displayed
			** "Initialized empty Git repository in /Users/<userName>/git-102/.git" ** 

Inorder to make the Git concept clear enough , we should create a sample projet. The sample project has two file of html and css. The name of the files are as follow.
# index.html 
# style.css

# git status 
It shows the status of the branch. The message from the **git status** will tell you about what changes have been made on the branch, and not yet commited or untracked. It puts the files in color red or green.
	**red  file**
		colored files are those not tracket.
		
# git add 
It is a command which will make the file to add to the respository. The applicaiton of the git add is as folloe
	**git add "<fileName>"**	
	Looking again  through a command **git status** will show the following message
	On branch master

	No commits yet

		Changes to be committed:
 			 (use "git rm --cached <file>..." to unstage)

		new file:   index.html


# git rm --cached <fileName>"
This is a command which is useful to unstage the change alreay added to the fiel from the latest git add. this will make the content to be one verion less from the last added feature.
	rm 'index.html'
	looking back again the git status , it will show the following result  
	On branch master

	No commits yet
	Untracked files:
 		 (use "git add <file>..." to include in what will be committed)
		index.html
	nothing added to commit but untracked files present (use "git add" to track)
	

# git commit -m "message use a title of commit "
This is a command used to commit the chnage already added to the local repository. The applciaiton of the command is as follow
	**git commit -m "commit messge"**
	[master (root-commit) 773db17] Add header
 	1 file changed, 10 insertions(+)
 	create mode 100644 index.html
	
	
