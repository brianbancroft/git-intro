# MAPTIME Introduction to Git
An Introduction to Git

Date: Tuesday, January 24, 2017 - 18:45

# What
Versioning. It's that thing you can do with your files to ensure that you (and your peers) can collaborate on the same project, while being able to access prior versions of the topic at any given notice. 

It's like an unlimited undo, and it also allows large groups of people to work on the same thing at once. 

For this evening, we're going to 

* Give a brief overview on what versioning is
* Set up Git on your machine
* Create a Repository
* Tracking Changes; or `add`, `commit`, `log`
* Recover old Changes
* Collaborating
* Conflicts
* The Leaflet Map Exercise
* Bonus: The Gitignore


This is going to be a lecture that's geared to teach 

# Why
Developers use versioning so that they can collaborate, share and exchange ideas with the minimum amount of fuss possible. You're going to learn it so that you all can 

# What you're going to need to do well

* Your own laptop
* An Internet connection
* A chipper attitude to learn something that's tricky at first


# Setup

To Access the Ryerson Wifi, you'll need the following: 
_Note to self: Get Ryerson public wifi info on monday in advance_

Chances are if you're running a newer mac, you'll already have Git installed. If you don't, you can a suitable downloader here:
https://git-scm.com/downloads


# Theory

While many are working on setup, here's a quick rundown on what Git is. 

<! 5 minutes maximum >


# Setup - Continued

Once you've installed git, you're going to need to open the command line tools. This is `Terminal` in Linux/Mac, or Dos in Windows (There is also the git bash as well)

The first thing you should do when you install git is to set up your user name and email address. This allows you inject your identity into your commits. 

```
git config --global user.name "Brian Bancroft"
git config --global user.email hello@brianbancroft.ca
```
There are some other settings that I will be glossing over including the default editor which git uses, as this will be out of scope with the time available tonight. 

To see whether you've entered the proper user name or email, type in the following:
```
git config user.name
git config user.email
```
If you've made a mistake, all you have to do is re-enter the configuration variables as we just did above. 

# Initializing Repos, Adding files and committing
The next potion will be rapid-fire. Now that we've set up Git, we're going into the basic mechanics of versioning your work, on your own. 


## Initializing a Repos
In order to create a new repo, the command used is `git init`. 



To make use of that command, do the following: 

1. In the command prompt or terminal, navagate to the directory by using the following commands:
  - `cd <directory name>` for all operating systems
  - `cd ..` to go back a directory
  - `ls` (linux, mac) or `cd` (windows) to see the contents of your directory. 
2. Before we initialize the repository, we want to verify the repo's status. Enter `git status` to verify.
3. Once in the proper directory, type in `git init`. This initializes the repository. 

### Git status
`git status` shows the status of your repo including changes that are staged, or unstaged. 

## Commiting to a Changes
When you've made changes to a file or a series of files, there are two commands you need to do to version them:

1. `git add <filename>` or `git add .`, which adds one or more files. 
2. If you're sure that you want to _commit them_, use `git commit -m <message here>`

When you type in a commit message, try to keep it under 50 characters, short, and in the present tense.

## Undoing your last set of Changes

## Looking at a log

## Jumping to a certain point in the log. 

# Sharing and Collaborating

In this section, we're going to now take what we've learned on our own and expand using tool for collaboration. While we can store repositories locally, there are places where we can store and share these repositories among other users. These tools include Github, Bitbucket and Gitlab. 

Because it is currently the largest home to most open-source projects, we're going to collaborate on Github. 

## Branches

### Creating new Branches

### Switching

### Rebasing

### Merge

## Conflicts

# Online Collaboration

## Theory: Difference between Git and Github

### Creating a Repo and setting it up

### Cloning a Repo

### Best Collaboration: The Pull Request

Sometimes when collaborating, it's entirely possible to run into conflicts with your source material. 

# Leaflet Exercise
So this is the last portion. Because Maptime is about the intersection of mapping and the internet, it wouldn't feel right to finish the night without putting our hands on a map 

`git clone <insert repo for maptime leaflet example here>`

####
Source Material: 
http://swcarpentry.github.io/git-novice/
Copyright © Software Carpentry 
