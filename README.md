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

------------------------------------------Repository------------------------------------------- 

Essentially git repository is a directory called ".git" inside of your project.
This repository tracks all the changes made to your project's files, building up a history over time.


--------------------------------------------Commit---------------------------------------------


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





