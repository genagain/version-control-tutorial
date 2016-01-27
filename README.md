# Version Control Tutorial

This is a repository to teach the basics of version control. A repository is a central location where all the code is stored for a given project.

## Installation
Before you can do anything, we need to install git, which is a command line utility for version control. It integrates seamlessly with Github.

[Here](https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/) is a tutorial on how to do this. This tutorial goes in to more detail on installing other things besides git and integrating it with Github, so stop after you've completed step 4.

## Cloning

Cloning is when one copies the entire contents of a repository on to their computer. Once you clone a repository, you can work with it on your computer.

To clone this repository, we run the following command in your terminal:
```
git clone https://github.com/genagain/version-control-tutorial.git
```

By running this command, we are using the HTTPS protocol. This is form of the HTTP protocol which is run on top of the SSL protocal.

## Go to directory

In layman's terms, a directory is a folder

```
cd version-control-tutorial
```

## Make a branch

![Representation of version control](https://jonasatwork.github.io/gitPresentationAssets/git-branch.png)

```
git checkout -b YOUR_BRANCH_NAME
```

## Edit Files

Here is when you make the changes and addition necessary to create your project!

## Add Files

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

* Go to this Github repository in your browser
* Click on this branch
* Click create pull request
* Review all of the changes you made

Merge Branch

Deal with Merge Conflicts
