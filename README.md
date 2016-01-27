# Version Control Tutorial

This is a repository to teach the basics of version control. A repository is a central location where all the code is stored for a given project.

## Installation
Before you can do anything, we need to install git, which is a command line utility for version control. It integrates seamlessly with Github.

[Here](https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/) is a tutorial on how to do this. This tutorial goes in to more detail on installing other things besides git and integrating it with Github, so stop after you've completed step 4.

## Cloning

Cloning is when one copies the entire contents of a repository on to their computer. 


To clone this repository, we run the following command in your terminal:
```
git clone
```

By running this command, we are using the HTTPS protocol. This is form of the HTTP protocol which is run on top of SSL.

## Go to directory

```
cd 
```

Make a branch

```
git checkout -b YOUR_BRANCH_NAME
```

Edit Files

Add Files

```
git add .
```

Make a commit

```
git commit -m "YOU MESSAGE GOES HERE"
```

Repeat

Push Branch

```
git push origin YOUR_BRANCH_NAME
```

Create pull request

Merge Branch

Deal with Merge Conflicts
