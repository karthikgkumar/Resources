# What is Git?

## What is git and why is it around?

Git is the most commonly used version control system. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source. So regardless of whether you write code that only you will see, or work as part of a team, Git will be useful for you.

&#x20;

<figure><img src="../../.gitbook/assets/5b9f81f6 2230 4ca8 b8a7 cf005b98eba5.png" alt=""><figcaption></figcaption></figure>

## What is a Version Control System and what are its uses?

Version control systems are a category of software tools that helps in recording changes made to files by keeping a track of modifications done in the code.

#### Uses

> A repository: It can be thought of as a database of changes. It contains all the edits and historical versions (snapshots) of the project.

> Copy of Work (sometimes called as checkout): It is the personal copy of all the files in a project. You can edit this copy, without affecting the work of others and you can finally commit your changes to a repository when you are done making your changes.

> Working in a group: Consider yourself working in a company where you are asked to work on some live project. You can't change the main code as it is in production, and any change may cause inconvenience to the user, also you are working in a team so you need to collaborate with your team to adapt their changes. Version control helps you with merging different requests to the main repository without making any undesirable changes.&#x20;

## History of Version control system

### Types of Version Control Systems:

* Local Version Control Systems
* Centralized Version Control Systems
* Distributed Version Control Systems

#### Local VCS

It is one of the simplest forms and has a database that kept all the changes to files under revision control. RCS is one of the most common VCS tools. It keeps patch sets (differences between files) in a special format on disk. By adding up all the patches it can then re-create what any file looked like at any point in time. The System will prompt the user for installing the software.You can give "Yes" for installing it. Disadvantage is that You will lose everything if your hardware malfunctions. :::

#### Centralised VCS

Centralized version control systems contain just one repository globally and every user needs to commit for reflecting one's changes in the repository. It is possible for others to see your changes by updating.

![image.png](<../../.gitbook/assets/0aba2e12 7030 46cf 91dc 36b3df203a1a.png>)

What if the hard disk of the central database becomes corrupted, and proper backups haven't been kept? You lose absolutely everything. Due to this disadvantage,we came up with an idea of Distributed VCS.

#### Distributed VCS

Distributed version control systems contain multiple repositories. Each user has their own repository and working copy.Just committing your changes will not give others access to your changes. This is because commits will reflect those changes in your local repository and you need to push them in order to make them visible on the central repository. Similarly, When you update, you do not get others' changes unless you have first pulled those changes into your repository.

&#x20;

<figure><img src="../../.gitbook/assets/009ae35b c246 439c b5b4 37e60852b22b.png" alt=""><figcaption></figcaption></figure>

#### How was Git created?

As with many great things in life, Git began with a bit of creative destruction and fiery controversy. The Linux kernel is an open source software project of fairly large scope. For most of the lifetime of the Linux kernel maintenance (1991--2002), changes to the software were passed around as patches and archived files. In 2002, the Linux kernel project began using a proprietary DVCS called BitKeeper. In 2005, the relationship between the community that developed the Linux kernel and the commercial company that developed BitKeeper broke down, and the tool's free-of-charge status was revoked. This prompted the Linux development community (and in particular Linus Torvalds, the creator of Linux) to develop their own tool based on some of the lessons they learned while using BitKeeper. Some of the goals of the new system were as follows:

* Speed
* Simple design
* Strong support for non-linear development (thousands of parallel branches)
* Fully distributed
* Able to handle large projects like the Linux kernel efficiently (speed and data size) Since its birth in 2005, Git has evolved and matured to be easy to use and yet retain these initial qualities. It's incredibly fast, it's very efficient with large projects, and it has an incredible branching system for non-linear development.

#### GIT FEATURES

* Tracks history
* Free and open source
* Supports non-linear development
* Creates backups
* Scalable
* Supports collaboration
* Branching is easier
* Distributed development

## GIT THREE STAGE ARCHITECTURE

![image.png](<../../.gitbook/assets/3864626d 517e 4e77 b1f4 8452ca1da9f4.png>)

* Git directory - stores the metadata and object database for your project.It is what that is copied when you clone a repository from another computer.
* Working directory- Single checkout of one version of the project. The files are pulled out of the compressed database in the Git directory and placed on disk for you to use or modify.
* Staging area -It is a simple file that is present in your git directory,that stores information about what will go into your next commit.

## GIT COMMANDS

#### Different Commands in Git

* Git config
* Git init
* Git add
* Git diff
* Git commit
* Git reset
* Git status
* Git merge
* Git push
* Git pull

### Git config

#### To set Globally

* Open the command line/git bash/any terminal.
* Set your username: `<span style="color:red">`{=html} git config --global user.name "Name"`</span>`{=html}
* Set your email address: `<span style="color:red">`{=html} git config --global user.email "[MY\_NAME@example.com](mailto:MY\_NAME@example.com)"`</span>`{=html}
* Type your name and email address in the above string part.
* Verify your configuration by displaying your configuration file: `<span style="color:red">`{=html} Git config --list`</span>`{=html}

#### To set repository-specific username/email configuration:

From the command line, change into the repository directory. Set your username: git config user.name "FIRST\_NAME LAST\_NAME" Set your email address: git config user.email "[MY\_NAME@example.com](mailto:MY\_NAME@example.com)" Verify your configuration by displaying your configuration file: Git config --list.

### git init

This command is used to initialize a git repository.

* Let's check the current working directory:
  * `<span style="color:red">`{=html} pwd`</span>`{=html}
* To create a repository in the working directory, use the following commands:
  * `<span style="color:red">`{=html} mkdir demogit `</span>`{=html}
  * `<span style="color:red">`{=html} cd demogit`</span>`{=html}
  * `<span style="color:red">`{=html} pwd`</span>`{=html}
* The directory "demogit" will be empty for now.
* Let's create a folder for the repository.
  * mkdir firstRepo
  * cd firstRepo
  * pwd
* The folder "FirstRepo" is empty. We will now initialize a repository to our folder.
* If we check git status, we could see that currently git is not initialized.
* Now we will git init

![image.png](<../../.gitbook/assets/ca1e80bc f030 4fc0 9717 1026fcfd1375.png>)

When we add git init,Something called the "master" appears on the screen. Whenever a Git repository is created for the first time, it creates a branch, and the name of the branch is master.

![image.png](<../../.gitbook/assets/3da0cf6a 5670 47f7 a6c0 ad9d5ff5b697.png>)

Navigate to the folder; you can find a hidden ".git" folder. If you check the folder, you can see several directories and configurations. Make sure you don't make any changes to any of the directories.

&#x20;

<figure><img src="../../.gitbook/assets/fe0a8f4d a897 4300 b168 2a888433487b.png" alt=""><figcaption></figcaption></figure>

### git add AND git commit

Moving further, let's make some commits. For that, I will create two notepads and commit them one by one.

For the first notepad, the commands are as follows: touch fossmec.txt notepad fossmec.txt

### git status

Next, let's check the status of the file that was created.

git status

This shows that there isn't a file committed yet, and there are untracked files. The untracked files can be seen in red.&#x20;

### git add

For Git to track that file, add command is used. If you know the exact name of the file, you can specify it or else you could simply type the following command: git add --all&#x20;

<figure><img src="../../.gitbook/assets/964cb379 de5a 490c a845 2dbcfac269c2.png" alt=""><figcaption></figcaption></figure>

You could see that the file is now in the staging area,so it's shown in green colour. The next step is to commit the file. git commit -m "fossmec"

Let's check the status of the file again.&#x20;

You'll notice that there are no more commits to be made, as there was a single notepad and that was committed in the previous step.

Next, check all the information regarding the commits that were made. git log&#x20;

<figure><img src="../../.gitbook/assets/0e74ac68 d66e 4cf6 b86f 764da7ca4f97.png" alt=""><figcaption></figcaption></figure>

This displays the commit ID, author's name, and email ID used. You can also find the date and commit message on the screen. Let's make one more commit.

Repeat the same process again. ie to make a notepad, add something to it, and close it

### DIFFERENCE BETWEEN GIT ADD. AND GIT ADD --ALL <a href="#difference-between-git-add-and-git-add-all" id="difference-between-git-add-and-git-add-all"></a>

Git Add -a Command "git add -A" stages all the changes. It is equivalent to "git add -all" or "git add . , git add -u" combined. Here, we will understand the difference between both of them as follows.

* "git add ." stages new files and modifications, without deletions (on the current directory and its subdirectories).
* "git add -u" stages modifications and deletion without new files.
* So, "git add -A" is a handy shortcut to both of those.

> git add -A

> git add -all

> git add . git add -u

### ACTIVITY 1

* Create a text file named git\_tutorial.txt and add one thing that you learnt today.
* Commit the changes and create second version
* Look at the git logs&#x20;

Now, let's push the two notepads on GitHub.Open your GitHub account, and create a new repository. The name of the repository will be "FirstRepo." Copy the "git remote add origin" URL.

### Homework 1

1. Create an empty folder and initialize a local repository.What was added to your folder?
2. Create a file myname.txt and fill in your name on the first line.
3. Add the file to the staging area and then commit to add it in the local database.
4. Track the .git directory by noticing the changes in it as you add files and make commits locally.
5. Create a college.txt and fill in your college name.Also create a newyear.txt and add one of your new year Resolutions.
6. Delete myname.txt
7. Add college.txt to staging area and commit.
8. Track changes
9. Checkout to previous version&#x20;

### GIT BRANCH

#### BRANCH

A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project.

![image.png](<../../.gitbook/assets/d9ebe1e8 3cdb 4580 b183 2b3f195c1918.png>)

The above scenario

now let's add hello.txt,thanks.txt,index.txt,hai.ppt and a directory new

![image.png](<../../.gitbook/assets/d6567e16 a878 42f7 8660 7623fb00ee62.png>)

commiting the changes, we have our initial commit.

![image.png](<../../.gitbook/assets/6743fdb6 d2ba 4126 8797 33dd14fd883c.png>)

A new branch dev is created and also we are checkedout to that branch using the following code

![image.png](<../../.gitbook/assets/8b6159f6 98df 4b36 9378 69b88e80372b.png>)

I am adding changes to index.txt and thanks.txt

![image.png](<../../.gitbook/assets/cd7a1405 b9b4 4ec4 96e0 aa4d87e9df9a.png>)

Deleting some files

![image.png](<../../.gitbook/assets/015712d6 d62c 4c89 99c1 d68a954b05e1.png>)

Folder structure is given below for the dev branch

![image.png](<../../.gitbook/assets/79a0441c ed9a 42a3 995e b8d94a4ee778.png>)

The changes are committed and we checked out to the master branch.

![image.png](<../../.gitbook/assets/152ddda7 db3a 4426 aac4 b7691f389022.png>)

The folder structure of master branch:-

![image.png](<../../.gitbook/assets/70450740 7ecd 43b6 b9ed d066ae57e4b3.png>)

The above example shows the implementation of how branches are used.

COMMON OPTIONS

* git branch List all of the branches in your repository. This is synonymous with git branch --list.

$ git branch `<branch>`{=html} Create a new branch called ＜branch＞. This does not check out the new branch.

$ git branch -d `<branch>`{=html} $ Delete the specified branch. This is a "safe" operation in that Git prevents you from deleting the branch if it has unmerged changes.

$ git branch -D `<branch>`{=html} $ Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.

$ git branch -m `<branch>`{=html} $ Rename the current branch to ＜branch＞.

Delete a Remote Branch You can delete a remote branch from Git desktop application. Below command is used to delete a remote branch:

$ git push origin -delete `<branch name>`{=html} $

Switch Branch Git allows you to switch between the branches without making a commit. You can switch between two branches with the git checkout command. To switch between the branches, below command is used:

$ git checkout`<branch name>`{=html} $ Switch from master Branch

You can switch from master to any other branch available on your repository without making any commit.

Syntax:

$ git checkout `<branch name>`{=html} $

As you can see in the output, branches are switched from master to branch4 without making any commit.

Switch to master branch.You can switch to the master branch from any other branch with the help of below command.

`$ git branch -m master $`

Merge Branch Git allows you to merge the other branch with the currently active branch. You can merge two branches with the help of git merge command. Below command is used to merge the branches:

```bash
$ git merge <branch name>{=html} $ List all remote branches.
$ git branch -a
```

Creating Branches It's important to understand that branches are just pointers to commits. When you create a branch, all Git needs to do is create a new pointer, it doesn't change the repository in any other way.

### Git Merge and Merge Conflict

In Git, the merging is a procedure to connect the forked history. It joins two or more development history together. The git merge command facilitates you to take the data created by git branch and integrate them into a single branch. Git merge will associate a series of commits into one unified history. Generally, git merge is used to combine two branches.

It is used to maintain distinct lines of development; at some stage, you want to merge the changes in one branch. It is essential to understand how merging works in Git.

In the above figure, there are two branches master and feature. We can see that we made some commits in both functionality and master branch, and merge them. It works as a pointer. It will find a common base commit between branches. Once Git finds a shared base commit, it will create a new "merge commit." It combines the changes of each queued merge commit sequence.

The "git merge" command The git merge command is used to merge the branches.

#### Fast Forward Merge

If we change our example so no new commits were made to the base branch since our branch was created, Git can do something called a "Fast Forward Merge". This is the same as a Merge but does not create a merge commit.

This is as if you made the commits directly on the base branch. The idea is because no changes were made to the base branch there's no need to capture a branch had occurred

![image.png](<../../.gitbook/assets/c4f3d424 d069 4858 a742 9bebfdf92b96.png>)

#### Resolving Merge Conflict

**When Merge Conflicts happen?**

When you merge branches that have competing commits, and Git cannot decide which changes to incorporate in the final merge, that's when merge conflicts happen.

**Resolving Conflicts:**

There are many ways to resolve conflicts on Git Merge. But we are going to use the easiest one. By using VSCode. Just Install VS Code in your system and open those files who have conflicts, and you will see 2 options: Current Change and Incoming change. Just like this.

Just choose Accept Incoming change. Save the file and commit the files by typing "git add .", and "git commit -m "message" ". Now you have successfully merged 2 branches.

![image.png](<../../.gitbook/assets/a4a811d1 7f07 4fd5 8a78 f20fc2a13bf0.png>)

Let's see when the conflict occurs

To see the merge log

![image.png](<../../.gitbook/assets/923a671f 8555 4bc0 a39c 4e8601ef3c91.png>)

#### Branch Management:

We can create many branches in our repository and work in them. We also need to manage them. So let's see few commands for managing branches in Git:

* To see all the branches you have created you will need to use this command : "git branch" and the current branch will have "\*" in front of the branch.
* To see Branches and that branch's last commit along with it's message type "git branch -v" and press enter.
* If you want to see which branches were merged then use "git branch --merged" and those that were not merged use "git branch --unmerged".
