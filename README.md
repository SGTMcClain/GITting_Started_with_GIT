# GITting Started with GIT
- [GITting Started with GIT](#gitting-started-with-git)
  * [What is GIT?](#what-is-git)
  * [What is Github](#what-is-github)
  * [Installing Git](#installing-git)
  * [Installing Github Desktop](#installing-github-desktop)
  * [Installing Git-LFS](#installing-git-lfs)
    + [Why do we need to do this?](#why-do-we-need-to-do-this)
  * [Start_Unity_Github_Project](#start-unity-github-project)

## What is GIT
Git is a free and open source distributed version control system. This means that there is a remote repository and local repositories on each developer’s computer. Each developer can modify their local branch and commit (save) it locally then push their code back to the remote repository. Once code is in the remote repository other developers can pull those changes into their local repository to keep their local repository up to date with the remote repository. Git also keeps a history of all of the changes made to the repository so that nothing is ever truly lost so long as it is committed. This whitepaper will cover of some of the basics of using Git.

## What is Github
According to [Github.com](https://guides.github.com/activities/hello-world/) GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

During our class Github will also be known as the remote repository.

Github is a complete DevOps platform based around git source control management (SCM). Gitlab serves as the host for our git remote repository and it also provides a web based graphical user interface (GUI) to visualize what our Git looks like. We can use the GitLab platform to navigate branches, manage merge/pull requests, manage packages, store release binaries and a whole lot more.

## Installing Git
This is the software that run git.  It is command line only so it can be a bit intimidating to use at first but to get around this we will also install Github Desktop to make things a bit easier.

1. Download Git from https://git-scm.com/downloads
2. Install Git onto your machine
    1. On the step where it asks you about default editors select either Notepad++ or Visual Studio Code
3. Confirm that you have successfully installed Git by going to your command prompt (console on Mac) or using GitBash which was just installed and run the command

    ```git --version```
    
    This command should return the current version of Git
    
## Installing Github Desktop
1. Download Github Desktop from https://desktop.github.com/

## Installing Git-LFS
Because we are using Unity we need an addon that will help us manage large binary files like pictures, 3D models, and audio files.
LFS stands for Large File Storage.  With this add-on installed we can utilize a text file to manage what files LFS should save instead of saving them to git.

You can download and install Git-LFS here https://git-lfs.github.com/

### Why do we need to do this
Git manages text files very well and technically any file that you save to your computer can be viewed as some form of text file.  This is great for Readme.md files and code files because they are usually made up of only text.  However larger files like pictures, 3D models, and audio files are massive in size which also means that they would be huge to keep track of.  These files also may have small portions that change everytime the file is opened which can give git fits about what the correct version is.  LFS keeps track of these changes seperately from Git so that it doesn't cause any larger issues (Merge Conflicts). 

## Start Unity Github Project
Use this template to start a Unity3D project using Git and Github. 

The goal of this repository is to make it easy to get started with source control in Unity.  

The article in the link below explains why git is difficult, but not impossible, to use with unity with git and how you can setup your project to be a bit more "git" friendly [How to Git with Unity](https://thoughtbot.com/blog/how-to-git-with-unity)

The following directions assume that you have github desktop [[Download Here]](https://desktop.github.com/) and git-lfs[[Download Here]](https://git-lfs.github.com/) already installed on your computer, as well as having a github account.  I will also assume that if you are familar with git/github and use either the command line or a GUI other that github desktop you should be okay without step by step instructions.

Once you are ready:

1. Click "Clone or Download"
2. Click "Open in Desktop".  This will open the Github Desktop application
3. Select a folder on your system and Click "Clone"
4. Open the new folder with this README.md in your file manager
5. Copy your existing Unity project folder into this folder
6. Go back to Github Desktop and create a commit message, then Click "Commit"
7. Once the commit is complete Click "Push"

If your Library folder is not being ignored open your command line tool in your this folder and run:

`git rm -r --cached Library`

then

`git commit -m "Removed Library Folder from repository"`
