#In this project we learn how to use Git.

Step 1) git init <folderNameForLocalRepo>
Step 2) Create any file like README.md
Step 3) git status
Step 4) git add <filename or .>
Step 5) git commit -m "<message to commit to local directory>"
Step 6) Type "git remote -v" to check if this local directory is linked to some remote directory on github or not.
Step 7) Create a remote repository on Github where you want to link your local repo
Step 8) To link remote repo to local, type "git remote add origin <link of repo>". origin is basically the name of remote reference. We can change this as per convenience but default is used in general.
Step 9) To put data on remote reference from local, type "git push -u origin master". The -u parameter is used to create a tracking relation between what is locally my master and my origin.

Now since a new branch has been created on the github by the name master, subsequent push command will not require "-u"

Step 10) Connecting github using SSH. This is specially used to avoid entering username password at each push. Following steps are used to create SSH keys, add it to agent and configure that key into our GitHub account-
	a) ssh-keygen -t rsa -b 4096 -C "chahat.bansal@cse.iitd.ac.in" 
	b) Enter the file in which to save the key
	c) Enter a passphrase for extra security (you can actually keep it empty and just press Enter)
	d) Press Enter
	e) Go to the file path mentioned above and copy the ssh key. 
	f) Open the github repository and in settings to the "SSH and GPG keys", there press "New SSH key", give it a name, and then press Enter.
	g) To test if it is working correctly, on terminal type- "ssh -T git@github.com"

Step 11) git clone <ssh/html url from github>: A clone command makes a full copy (including all branches and tracking) of remote repo into your local repo.

Step ) Git Fetch: used to fetch changes from the remote repo. This should be usually done before any push command is given. 

Step ) Git Merge: used to automatically (or manually) merge the changes fetched from remote repo with your local repo. This should be usually done before any push command is given.

Step ) Git pull: This can be done as a shortcut to do the work of fetch and pull. 

##Knowing about README file
README file should contain information like what the project does, how it can help the project, who owns it, and so on. README file is written in MarkDown i.e. md font. markdown means that it can be converted into HTML easily.	

##Knowing about CONTRIBUTING.md file
This file can be used to write some message or set some guidlines for the contributors of this project.

"This text is to test the fetch, merge, and pull command".

