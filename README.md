#GITting Started with GIT

## What is GIT?
Git is a free and open source distributed version control system. This means that there is a remote repository and local repositories on each developer’s computer. Each developer can modify their local branch and commit (save) it locally then push their code back to the remote repository. Once code is in the remote repository other developers can pull those changes into their local repository to keep their local repository up to date with the remote repository. Git also keeps a history of all of the changes made to the repository so that nothing is ever truly lost so long as it is committed. This whitepaper will cover of some of the basics of using Git.

## What is Github
According to [Github.com](https://guides.github.com/activities/hello-world/) GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

During our class Github will also be known as the remote repository.

## Installing Git
1. Download Git from https://git-scm.com/downloads
2. Install Git onto your machine
    1. On the step where it asks you about default editors select either Notepad++ or Visual Studio Code
3. Confirm that you have successfully installed Git by going to your command prompt (console on Mac) or using GitBash which was just installed and run the command

    ```git --version```
    
    This command should return the current version of Git
    
## Installing Github Desktop


## Start_Unity_Github_Project
Use this template to start a Unity3D project using Git and Github. 

The goal of this repository is to make it easy to get started with source control in Unity.  

The article in the link below explains why git is difficult, but not impossible, to use with unity with git and how you can setup your project to be a bit more "git" friendly [How to Git with Unity](https://thoughtbot.com/blog/how-to-git-with-unity)

The following directions assume that you have github desktop [[Download Here]](https://desktop.github.com/) and git-lfs[[Download Here]](https://git-lfs.github.com/) already installed on your computer, as well as having a github account.  I will also assume that if you are familar with git/github and use either the command line or a GUI other that github desktop you should be okay without step by step instructions.

Once you are ready:

1. Click the "Use this template" button on this page. This will create a new repository in your account
2. Give This repository a name related to your game
3. Click "Create repository from template"
4. Click "Clone or Download"
5. Click "Open in Desktop".  This will open the Github Desktop application
6. Select a folder on your system and Click "Clone"
7. Open the new folder with this README.md in your file manager
8. Copy your existing Unity project folder into this folder
9. Go back to Github Desktop and create a commit message, then Click "Commit"
10. Once the commit is complete Click "Push"

If your Library folder is not being ignored open your command line tool in your this folder and run:

`git rm -r --cached Library`

then

`git commit -m "Removed Library Folder from repository"`
