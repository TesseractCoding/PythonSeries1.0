# I am just GITING :bulb:

### Git commands in use:
#### Git Branch

In Git, branches are a part of your everyday development process. Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes. This makes it harder for unstable code to get merged into the main code base, and it gives you the chance to clean up your future's history before merging it into the main branch.

#### Git Checkout

In Git terms, a "checkout" is the act of switching between different versions of a target entity. The git checkout command operates upon three distinct entities: files, commits, and branches. In addition to the definition of "checkout" the phrase "checking out" is commonly used to imply the act of executing the git checkout command. In the Undoing Changes topic, we saw how git checkout can be used to view old commits. The focus for the majority of this document will be checkout operations on branches.

The git checkout command lets you navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch. Think of it as a way to select which line of development you’re working on.
***

### Testing Assignment submission :wink: 

```console
git clone https://github.com/TesseractCoding/PythonSeries1.0.git
cd PythonSeries1.0/Day2/submission_test
git branch <new branch name>[this should be your first and last name, for eg. for me 'Vinamra Munot']
git checkout <new branch name>
```

> makes changes required, this might include making new files, modifying files & deleting files
>
> make a file named "test.py" and write print('hello world')

```console
git add test.py
git commit -m "testing branch changes"
git push -u origin <name of the branch>
```


# :feet: Congrats You are officially Tesseract Coders :octocat:
