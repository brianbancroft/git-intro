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

## Commiting to a Changes

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
