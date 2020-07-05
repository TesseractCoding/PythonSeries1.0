# I am just GITING :bulb:

## Why is git/vcs important?

<p style="text-align: center"> One of the key principles is to continuously plan, build and release small improvements to your project/product. As the name suggests <strong><mark>Version Control System</mark></strong>, we use this tool to create history of our project. In other words, we create small upgrades to your product to improve it step by step.
</p>
<p> Some might also refer this as a <strong>snapshot</strong> :camera: &nbsp of the project/product at a given point of time. </p>


<p align="center"><img src="readme_meme/snapshot-2.jpg" height="300" width="400"></p>


>> You ask why this is helpful?!

<p>This is the actual quantum mechanics at works. :unlock: &nbsp We can go back in time!! Yes you heard me right. The collection of commits contain the history of the project. I guarantee you can go back in time by choosing the version to go back to through labeling everything.
<br>
At any time you can review the project history and undo changes by going back to the previous part of the project. 
<br>
All the technicality is take care by git so you don't need to do anything. All you need to do is run commands and the rest taken care of, MOST of the time!
There is a lot of things in play here but first we are gonna concentrate on instantiating a git repo. </p>

## Why is open source important?

Open source is a type of licensing agreement that allows users to freely modify a work, use said work in new ways, integrate the work into a larger project or derive a new work based on the original. By removing barriers between innovators, open source promotes a free exchange of ideas within a community to drive creative, scientific and technological advancement.

Professionals utilize open source licenses in many industries: biotech, electronics, fashion, robotics and teaching to name a few. This article will focus exclusively on the software applications.

***

# Foundation of Git

it is a <strong><em>universal</em></strong> language. Github, GitLab and BitBucket are companies has adopted git open source project for its own company. 

In this module you will be learning how to setup git and use GitHub.

<hr>

## Git Installation

1. Visit [git-sm](https://git-scm.com/downloads "download link for git")
2. Choose the appropriate Download environment. For eg., I am using a Apple Laptop, thus I will be downloading Mac OS X package. You can choose either of the three depending on the operating system you have.

#### Check the git installation

> Open a Terminal/Powershell and enter `git --version`

```console
foo@bar:~$ git --version
git version 2.27.0
```
`If the installation is completed properly, you should receive a result with the version number otherwise it will tell you that no such module exists`

## Git Start
```markdown
                                                        Two ways
                                                         /    \
                                                        /      \
                                                       /        \
                                                    Cloning     Local
```

#### Git add

This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit. You must use the add command to add any new or modified files to the index.

#### Git commit

Create a new commit containing the current contents of the index and the given log message describing the changes. 

#### Git log

Shows the commit logs.

***

### MacOS/Linux/Windows

1. [Clone](#cloning-repo)
2. [Local](#local-terminal)

#### Cloning repo

- [ ] - Create a repo on github.com
- [ ] - ReadMe file

> As the name suggests __readme__, it meant to be read
<p align="center"><img src="readme_meme/readme.png"></p>

> you can clone the repo anywhere

```console
~$ git clone https://github.com/<github_username>/<reponame>
~$ cd <reponame>
~$ ls
Readme.md
```

#### Local terminal

- [ ] - Create a repo on github.com

```console
~$ mkdir <name>
~$ cd <name>
~$ git init
~$ git remote add origin https://github.com/<github_username>/<reponame>
~$ touch Readme.md
~$ echo "Hello World!" > Readme.md
~$ git add .
~$ git commit -m "something you wanna use to describe the change"
~$ git push -u origin master
```

```console
~$ git log
```

> The name of the folder and the name of the repo can be different. However, by default the name of the repo on github is clone everywhere

***

# :feet: Congrats You are an official OctaBabe! :octocat:

<p align="center"><img src="readme_meme/version.jpg"></p>

# Docs to read more

[Git Docs](https://git-scm.com/docs "Documentation of Git commands")

