# MAPTIME Introduction to Git
An Introduction to Git

Date: Tuesday, January 24, 2017 - 18:45

#HSLIDE 

# What is Versioning? 

![Background](img/phdComicsVersioning.gif)

#HSLIDE

## The plan:

* Give a brief overview on what versioning is
* Set up Git on your machine
* Create a Repository
* Tracking Changes; or `add`, `commit`, `log`
* Recover old Changes
* Collaborating
* Conflicts
* The Leaflet Map Exercise

#HSLIDE

# Setup

### Step 1: Get Wifi
To Access the Ryerson Wifi, you'll need the following: 
_Note to self: Get Ryerson public wifi info on monday in advance_
_ ensure wifi is on the presentation _

#HSLIDE

# Setup

### Step 2: Get Git and a Github Account!

(For all common platforms)
* GIT: https://git-scm.com/downloads

* Github: https://github.com

#HSLIDE

# Theory

While many are working on setup, here's a quick rundown on what Git is. 

<! 5 minutes maximum >

<Use lego block analogy>




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

What we've done is we've given your fingerprint and identity that explains who has changed what code.

# Initializing Repos, Adding files and committing
The next potion will about adding files, and commiting. Now that we've set up Git, we're going into the basic mechanics of versioning your work, on your own. 


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

The difference between the two is that adding one or more files sends it to a staging area, while commiting sends the information you've put together into the repository

When you type in a commit message, try to keep it under 50 characters, short, and in the present tense.

### Where do the old versions go?
They are stored on a _hidden_ directory, (.git/ for Mac and Linux users) so not to clutter up the system.

## Undoing your last set of Changes
If you've _added_ files that you want to undo, the command you seek is `git reset`. To reset a single file, it's `git reset HEAD <filename>`.

There are also circumstances where you want to revert your saving to the last commit. There are two commands which you should only use if you really need to. They are as follows:

1. `git reset --hard HEAD` for all files
2. `git checkout -- <filename>` if you only wish to revert a single file

Again, take *caution* when you use these, as you cannot recover what you've lost. 

## Logs and Diffs

If you wish to track the changes in a branch from the command line, you can use the command `git log`, which lists a series of commits.

If you wish to see the difference between one of more files which you've saved, but haven't committed, there's also the `git diff`. This command will show you the difference between what you've staged, and a prior commit. 



# Sharing and Collaborating

In this section, we're going to now take what we've learned on our own and expand using tool for collaboration. While we can store repositories locally, there are places where we can store and share these repositories among other users. These tools include Github, Bitbucket and Gitlab. 

Because it is currently the largest home to most open-source projects, we're going to collaborate on Github. 

## Branches

When you think of branches, it's easy to think of the branches of a tree, and how something can branch off from the main body. This isn't an incorrect way of thinking of it. 

Branches in git allow you to try new things, independently from the main source of the code without affecting the main code, until it is time to merge both branches of code. 


### Creating new Branches

To see all the available branches, type in `git branch`. 

### Switching

### Merge

## Conflicts

# Online Collaboration

## Theory: Difference between Git and Github

### Creating a Repo and setting it up

<Note to self - Skip Pair Programming and go straight to leaflet map> 

### Cloning a Repo

For this part, we want to show individuals 

### Best Collaboration: The Pull Request

Sometimes when collaborating, it's entirely possible to run into conflicts with your source material. 

# Leaflet Exercise
So this is the last portion. Because Maptime is about the intersection of mapping and the internet, it wouldn't feel right to finish the night without putting our hands on a map 

`git clone <insert repo for maptime leaflet example here>`

# Conclusion

Thanks for bearing with me for the last 1:20. What I've scratched is the basics of Git, and Github which are used widely by open source developers in both geospatial and non geospatial application. As you improve with these tools, as well as the command line, you'll find that there's a lot of ground to learn to use it in your day-to-day workflow. 

####
Source Material: 
This lesson was adapted from the Git Novice lesson from Software Carpentry. You can find the repo here:
http://swcarpentry.github.io/git-novice/
Copyright © Software Carpentry 
