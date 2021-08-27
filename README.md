# Intro-github-basics
Version Control System
# 1.0 VERSION CONTROL
Version control system is just a way to keep track of your codes or software for a layman explanationw I can called it a cloud drive but Totally different from drive but a some similar function as cloud drive because it helps to records and make changes to a file or sets of files that you can recall specific version later 
Some popular version control system include 

GitHub
Apache subversion
Mercurial 

With these you can clone some other repository of some others programmer codes into your Lab and lots more 

# 2.0 WHAT'S GIT 

Git is the most commonly used version control system among others. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source. 

So regardless of whether you write code that only you will see, or work as part of a team, Git will be useful for you.
N.B  GitHub is not git. Many people understandably confuse the two. GitHub is a website for hosting projects that use git.

Git is software that runs locally. Your files and their history are stored on your computer. You can also use online hosts (such as GitHub or Bitbucket) to store a copy of the files and their revision history. Having a centrally located place where you can upload your changes and download changes from others, enable you to collaborate more easily with other developers. Git can automatically merge the changes, so two people can even work on different parts of the same file and later merge those changes without loosing each other’s work!

Git is useful for coordinating work among multiple people on a project, and for tracking progress over time by saving “checkpoints”. You could use it while writing an essay, or to track changes to artwork and design files.

Git isn’t the only version control system out there, but it’s by far the most popular. Many software developers use git daily, and understanding how to use it can give a major boost to your resume.

Git is software that you can access via a command line (terminal), or a desktop app that has a GUI (graphical user interface)

# 3.0 PROCESS OF COMMITING A REPOSITORY TO GITHUB 

The first thing you'll need is a GitHub account, so head over and sign up. You'll also need git installed on your platform of choice. either window, mac or Linux but since am using linux I'll be showing you how to install git on your linux machine 
$ sudo apt-get update 
$ sudo apt-get install git 
doing this you've successfully install git on Kali Linux Machine 

# 3.1  How to create a new repository on GitHub

The first thing to be done is the creation of a new repository on GitHub. Log in to your GitHub account and go to the Dashboard. From that page click the Repositories tab. 
In the resulting window, give the project a name and an optional description. Depending on what this project is used for, you might make it private. 

Click Create Repository and GitHub will do it's thing. The address of the new repository will be:

https://github.com/Cyb3r-J0ll0f/InstinctHub​.git

How to connect your local project

Now the fun begins. On your local machine, create a new project folder with the command:

mkdir myproject

Change into that newly-created directory with the command:

cd myproject

Initialize the repository with the command:

git init

Now let's create a readme file with the command:

touch readme.txt

Add the new file to the staging area with the command:

git add .

Now we're going to create our first commit. If you're not sure what a commit is, it's simple: A commit adds the latest changes to the source code to the newly-created repository. These changes will then be part of the head revision of the repository.

To create the commit, issue the command:

git commit -m "added readme"

You can change the text in quotes to be whatever you want, such as "my first commit." Make sure the text in quotes describes what's been done for the commit.

The next step will make use of the GitHub repository address. What we need to do is add the local repository to the origin (the name of the remote repository where you want to publish your commits) of the remote repository. This is done with the command:

git remote add origin https://github.com/Cyb3r-J0ll0f/InstinctHub.git

At this point you can then push your work to the remote with the command:

git push -u origin master

When you run this command, you'll be asked for your GitHub username, followed by your GitHub user password. Upon successful authentication, your local repository will be connected to the remote GitHub repository and the readme.txt file pushed to the remote.


Push the changes to the master branch of the GitHub repository with the command:

git push -u origin master

Now, if you look at the repository on GitHub, you'll see the readme.txt
