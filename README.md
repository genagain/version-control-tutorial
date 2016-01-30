# Version Control Tutorial

This is a repository to teach the basics of version control. A repository is a central location where all the code is stored for a given project.

## Installation
Before you can do anything, we need to install git, which is a command line utility for version control. It integrates seamlessly with Github, which is a service for collaboarting on software.

[Here](https://desktop.github.com/) is a link to installing GitHub Desktop for Mac. In addition to, interacting with git through the command line, you can use a GUI as well.

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

Branches are a fundamental concept for version control. They allow people to work on the same software without using the same computer seamlessly. The picture below shows a representation of what version control is. **A branch consists of a series of incremental improvements in the development of the software.** In the picture below, every circle is one of these incremental improvements. The master branch is the copy of the software project that is always working as it should. In order to build features for the software project, people create a branch, which branches off from the master branch. This way when the person is incrementally improving the project, their changes will *not* affect the master branch. Once the feature is done and thoroughly tested it can be reincorporated into the project, which will be discussed later in this tutorial.

![Representation of version control](https://jonasatwork.github.io/gitPresentationAssets/git-branch.png)

To create a new branch, you run the command below:
```
git checkout -b YOUR-BRANCH-NAME
```

For example of you wanted to create a branch for the little feature you can run ```git checkout -b little-feature```

## Edit Files

Here is when you make the changes and additions necessary to create your project!

In this repository, there is a HTML file and two CCS files. The normalize.css file, is a file that ensures users using different browsers have a consistent experience when viewing a website. The style.css file is to style the the index.html file, which is empty.

You can do whatever you want to the index.html and style.css files. Remember to create new branches for any feature you want to create!

## Check the status

Throughout developing your software project, it's a good idea to check the status of your branch. This way you can be sure you know what is going on with your version control as you are developing the software.

To check the status of your branch, you run the following command:
```
git status
```

## Add Files

Basically after you make the changes you need to add them to be **staged**. Files that staged are can be part of an incremental improvement to your software, but are **not** yet. Staging is an concept that allows the user to decide which files will contribute to the incremental improvement. This concept is really useful because there is a chance that not all of the files you've change will contribute to your incremental improvement. 

To add all of you files that have changed, you run the following command:
```
git add .
```

To add individual files or directory, replace the period with the name of the file or directory.
```
git add NAME_OF_FILE_OR_DIRECTORY
```

## Make a commit

A commit is an incremental improvement to your software project. After you've added all of the changed files you want to staging, you can create a commit. Whenever you create a commit, it is expected that you write a message associated with it that clearly explains the changes you have made. This way you and other people can have an idea of the incremental improvements you've made to the software project. In the event that you mess up you can allows revert back to your most recent commit and pick up where you last left off.

To make a commit, you run the following command:
```
git commit -m "YOUR MESSAGE GOES HERE"
```

## Repeat

As you make more incremental improvements to your software project, make sure that you are adding and commiting each of them. The workflow is as follows: edit or create files, add files to staging, commit the change, repeat.

## Push Branch

When you are done with your feature, you push all of your changes to your branch. By doing this, all of the commits you've made on the branch can be incorporated in your software project. You are uploading all of the commits you've made on the branch to Github's cloud.

To push your branch, you run the following command:
```
git push origin YOUR_BRANCH_NAME
```

## Create pull request

Pull requests are where you and other people can review all of the changes you've made on your branch. You and other people can comment on certain lines of code. This way software developers can provide feedback for other people's code. Before your branch can be incorporated into your project you need to create a pull request.

To create a pull request, do the follow steps:
* Go to this Github repository in your browser
* Click create pull request for the branch
* Review all of the changes you made

It is important to note that you can continue to commit changes to this branch, after a pull request had been created. For example, you might want to make some more changes based on some feedback you've received for your pull request.

## Merge Branch

This is when you can incorporate your branch into your software project!

To merge your pull request, do the following steps:
* Go to this Github repository in your browser
* Click on pull requests
* Click on your pull request
* Click on "Merge Pull Request"
* Click on "Confirm Merge"

Now your branch as been incorporated into your software project!

## Deal with Merge Conflicts
Sometimes git isn't smart enough to figure what your software project will look like after a new branch has been merged. In this case you need to deal with each conflict individually. Because merge conflicts are hard to create on purpose, they are not included in this tutorial. If you want to learn to about merge conflicts you can read [this tutorial](https://help.github.com/articles/resolving-a-merge-conflict-from-the-command-line/)

## Pull down master

Now that you've incorporated your branch into the software project, you can start developing a new feature. To do this you need to update the copy of the software project on your computer to match what is in Github's cloud. This way your copy of the software project on your computer is the most recent working version of the software project. To do this we need to switch to the master branch of the project. 

To switch to the master branch, you run the following command:
```
git checkout master
```

Then you pull down the changes made to the master branch. This means you need to download the updated version of the master branch to your computer. 

To pull down the master branch, you run the following command:
```
git pull origin master
```

