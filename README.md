# LearningGit
this is a repository of notes that I use to learn the Git or GitHub language

https://www.youtube.com/playlist?list=PLcoYAcR89n-qbO7YAVj5S0alABLis_QVU 

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
