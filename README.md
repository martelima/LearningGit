# LearningGit
this is a repository of notes that I use to learn the Git or GitHub language

https://www.youtube.com/playlist?list=PLcoYAcR89n-qbO7YAVj5S0alABLis_QVU 

What is GIT?
Git is software for tracking changes to any set of files, generally used to coordinate work between programmers who develop source code collaboratively during during software development. Its objectives include speed, data integrity and support for non-linear distributed workflows.

Its objectives include speed, data integrity and support for for distributed non-linear workflows. This means that two or more people can work on the same project simultaneously, and in order to have historical control over what is being done, the tool allows you to have different versions of the code in different styles and/or functionalities.

but where would these projects be stored? which tool would help us work with Git? to answer this we can suggest GitHub, there are other tools on the market but this is one of the best known. so we can say that GitHub, Inc. is an Internet hosting provider for
software development and version control using Git. It offers distributed version control and the functionality of
Git's source code management functionality, as well as its own
features.

So in a nutshell we can say that GitHub has the functionality to store your project in a safe place, it allows you to share your project with other programmers, and other developers can collaborate with your project, there are many other possibilities, but we'll explore these later in this brief manual.

To understand this better, we need a few concepts:

## Repository

Essentially git repository is a directory called ".git" inside of your project.
This repository tracks all the changes made to your project's files, building up a history over time.

## Commit

Every "Commit" is a milestone in your project, i.e. when we launch some new functionality to the program or project it is interesting to make a Commit, there are cases where many commits are made for each code change, but depending on the need, it is interesting to adopt the idea of versioning, and each commit being a version like an update.

The example below is that each "@" represents a commit, in other words a milestone in a project's timeline.

       @--------------------------------@---------------------------------@------------>>>>
    start of                        Adding a                        Adding Whatsapp 
    project                       payment method                      integration

The interesting thing about versioning is that you can see how the project is changing and evolving, and you can return to a previous version that is more stable. 

to make a commit it is interesting to go through a few stages:

                        /Modified
               Commit--- Staging
                        \Committed

 
"Modified" would be the stage of modifying files, adding, deleting, editing, where Git records the modification. if you want to launch new lines in the Commit, we insert them in the staging stage, as a special area where it's already ready and just waiting to go live. So we can define that "Staging" represents the files ready to be sent. This stage is important for all the project developers to ensure that there is nothing to be corrected and that everything is in good working order. Once everything has been checked, it will be sent to the "Committed" stage, where the files will be inserted into the final version of the project. The ''Staging'' stage helps you to have a line of work and reliability in versioning, so let's say that it would be a stage more dedicated to testing and experimenting with routines.

Leaving aside "Commit", let's talk a little about "Branch", which is a branch of one of the historical points, usually aimed at a specific modification, which can return to the timeline or not. 

                                                    ----------@-------------@-------------------------@--------------------->
                                                   / 
                                   -----@----@----@-----                                      ------------@----------@------>
                                  /                     \                                    /
         @-----------------------@------------@----------@-----------------------------------@------------------------------>




Now that we've understood the basics of Git and GitHub, we need to install a Git terminal to learn and practise the commands. As a Windows user, I'd recommend the Cmdr programme (https://cmder.app/), as it's an excellent programme to start with and simple to use, but we recommend that you look for the one that best suits your needs and operating system.

After installing a git terminal on your computer, we can start testing some commands, we'll start identifying the version of git in the terminal using the command :
```bash
git --version
```                     
After checking the git version, let's make a configuration, type the following command into the terminal :     
```bash
git config --global --list
```
this line of code reports the settings that are inside git
And to enter our information into git we need to use a few commands, let's start by entering a username using the :
```bash
git config -- global user.name "YourName"
````
and to test whether the terminal has registered your username we use the command again:
```bash
git config --global --list
```
if you're following the steps correctly, you'll see after the previous command that the terminal now prints your username,  Now let's take advantage of this and enter the user's e-mail address using the command :
```bash
git config --global user.email yourname@yuoremail.com
```
we test it again with the command:
```bash
git config --global --list
```
now all commands registered from this point onwards will be identified by the terminal as having been carried out by a registered user

When we think about this tutorial we imagine that not everyone is used to the commands, so we'll briefly summarise some commands in the terminal to help you understand. So the first terminal command we should know is "ls" which means to list files and directories, If you create a file with notepad in this folder, when you ask the terminal to list it again, you'll notice that the end of the file ends with ".txt", which is the format of the text file. 

The second terminal command we need to learn is "cd", which means "choose directory". To test this, we recommend that you create a folder inside where your programme is installed, as the folder will act as a directory. Then type into the terminal "cd foldername/" 

When we execute this command, the terminal enters the folder you created, and if you type the command "ls" you'll realise that the terminal will list it, but as the folder is empty no files should appear.

then to create a file we'll use the command "touch TestFile.txt" after running this command, use "ls" to check that your text file has been created.

we believe that you may be annoyed by so much information in your terminal, so if you want to clear the information just type "clear"

ok! now that we know how to create and access folders or directories, create txt files, it's important to know how to remove them, in case you've created a file the wrong way round or want to clean up the folder we've created with the tutorial, use the "rm" command which means remove. As follows: "rm TestFile.txt"
attention !!! to remove folders and directories the command used is "rmdir"
to create directories the command is "mkdir NameChosen"

ok we know how to get into folders and directories, we know how to create and delete files, but we must also know how to get out of the folder we have created, so we use the command "cd ..", which returns us to the folder we were in before.

Now that we know how to navigate between directories, create and delete files, we can learn how to interact with files. To do this, we recommend that you create a directory and inside the directory create a text file, which we will interact with.
Now with the directory created where the file you created will be, use the command "nano TextFileName.txt".
Soon the terminal will change its appearance, as we open a text editor, where we have some tips below if we want to save, create pages, etc... and to use the commands just use the CTRL key with the letter corresponding to the functionality you want. .. let's go! be free and write a "Hello World!" and try saving through the terminal then check if it really worked!  To display the contents of the text file, simply use the command "cat TextFileName.txt"

##How to create your first repository:

we're going to create two folders named project-1 and project-02, we won't use project-2 because we're going to learn how to use a new command, to correct this deliberate error, start by opening the terminal and create the directories using: 
```bash
mkdir project-1
```
and then 
```bash
mkdir project-02
```
then check with the ‘ls’ command how the items in your directory are sorted
```bash
project-e2/ project-l/ testFi1e . txt
```
your terminal should probably show you the result we saw above, but don't worry, now we're going to learn the command ‘mv’ which means move, so type the following in the terminal :
```bash
mv project-02 project-2
```
