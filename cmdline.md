---
layout: default
---

# Command-line Course

This was a great course that aimed to demystify the seemingly opaque workings of \*NIX command-line. It started with basic navigation and progressed towards more advanced topics such as bash scripting and version control via Git. A variety of tools from text editors to commands such as `grep` and `sed` were introduced.

We also learned about corpus processing on the command line. It is fascinating how some things seem to be easier via the command line than by using some other tools or language. 

## Week 1: Introduction to Command Line Environments
During the first week we learned about command line environments and what they are all about. There are many/certain things that can be achieved faster and more easily via a command line than via a GUI. An example of this might be an installation of a program with a package manager.


## Week 2: Navigating the UNIX System
We learned about basic \*NIX navigation commands such as `cd`, `ls`, `pwd`, and others. We also learned about flags that one can append to certain commands. An example would be listing also the hidden files in a folder with `ls -a` instead of normal `ls`. We also learned about processes and how those could be monitored, managed, and killed. Then we learned to establish a connection to a remote server with `ssh`. Personally I had some problems with my CSC account and could not establish a connection, but connecting to a remote server is quite familiar to me from previous experience.

Here is a table that shows what the commands mentioned above do:

Command | What it does?
`cd` | Change to specified directory
`ls` | List the contents of current directory
`pwd`| Print the address of current directory
`ssh` | Establish a connection to a specified remote server

## Week 3: Basic Corpus Processing
This week we learned about `grep` and regular expressions as well as about standard streams. The most important thing I personally learned during this week was standard streams and how they can be utilised and/or directed around. It was also a good refresher on differences on DOS and \*NIX text files and regular expressions. This is the time that regex finally "clicked" in my head and it was quite easy to write them for the first time in my life.


## Week 4: Advanced Corpus Processing
Sed is the most important thing I learned about during this week. It is a powerful tool that can search, replace and modify text files with ease after one gets a hang of its quite peculiar syntax. It had been on my "I'll get to this later" list of things to look up, so it was a pleasant surprise that it was included in to the course curriculum. The next thing is probably to deepen my knowledge on `sed` and then to look up `awk` to accompany it. We also learned about the pipe `|` and about how it works.




## Week 5: Scripting and Configuration Files
This week we learned about bash scripting and about configuration files. One example of a bash sript was this one that we wrote for our assignment:

```bash
#!/usr/bin/env bash

filename=""
ls -a |
egrep "$1" > $filename

echo $filename
```

The script checks if a file exists in the current folder and prints out the name of the file if it exists.

Another thing about which we learned was configuration files. These files change the way our programs operate and we can modify those things to our liking. An example would be my Neovim config which lives in GitHub [here](https://github.com/ohtohalla/nvim-lsp-config).                                  

## Week 6: Installing and Running Programs
During this week we learned about installing and running programs on the command line. We also learned about permissions and how to manage them. Personally I had some problems when installing `blibparser` for python and it turned out there were some problems with the package at the time. It was still interesting to poke around and try to fix the problem. I learned some new things about permissions this week. Namely, I finally figured out how to parse the number codes of `chmod` without a reference. We also learned about Makefiles and their functions. THey make life significantly easier when storing things in version control or when sending a program to another person. Some things Makefiles help a user with are:

+ Managing dependencies
+ Lets user not clog version control with raw data
+ Makes cleanup easy after the files it helped to create are not needed anymore


## Week 7: Version Control
The las week was one that I had been waiting for, since it was about verison control and `git`. We learned the basics of Git and version control as a concept. I think this has provided me with enough understanding on the matter that I feel now comfortable to poke around a little more in Git and to finally try to figure out (among other things) what is the difference between _merging_ and _rebasing_. I also learned many things about Ruby On Rails since Jekyll was not comfortable with a newer version of Ruby that my OS happened to ship.

![](https://i.imgur.com/vPAiq.png)
