# Merge Conflicts
(breaking things up to fix them again)

## FEEL FREE TO DO THIS USING MY _Manbearpig_ repo (https://www.github.com/ricardoprins/manbearpig)

This step-by-step process will help you breaking things up and using a little bit of the git CLI magic to fix them up. As I said in the training, there are several other ways of messing up with VCS tools (a.k.a. GitHub) - this is just one of them.


We will simulate two people working in the same environment. Create a folder, and within that folder, create two different folders: A and B.

1. Using your favorite CLI interface, navigate to folders A and b and type `_git init A_` and `_git init B_` (if you can't get past this step, shoot yourself in the head and die.)
2. In directory A:
```
git remote add origin https://github.com/ricardoprins/manbearpig.git
(things will happen)
git pull origin master
(more things will happen)
```
3. In directory B, do the same thing that was done above.
4. Navigate to directory A, and in your lovely CLI interface, do the following:
```
touch ILOVEBREAKINGTHINGS.md
nano ILOVEBREAKINGTHINGS.md _(here, you can use your favorite text editor instead, or just type echo ILOVEBREAKINGTHINGS.md a - it should do the trick as well)_
_add a whole bunch of stuff to it_
git status
(you'll see information about what you've done with the tracked files)
git add .
git commit -m "Commit done from repo A"
git push origin master
```
5. Now let's change to directory B and try to do the same thing:
```
touch ILOVEBREAKINGTHINGS.md
nano ILOVEBREAKINGTHINGS.md
git add .
git commit -m "Commit done from repo B"
git push
```
ERROR!

Now, for the learning exercise: why did this happen? Try to ponder for a few seconds what just happened here, before we start trying to fix it.

---

Alright, if you've managed to understand what you just did, congratulations! You are one step ahead in the food chain!

So, how do we solve it?

First, a few considerations: 
Q: Are CLI or GUI tools the ideal ones to solve merge conflicts? 
A: It depends. There are situations in which you'll be able to solve stuff just from a GUI interface. However, if you know a bit more about git commands you'll be able to go through a wider set of problems, breezing through them!

Q: Do I REALLY need to use VCS tools? 
A: No, you don't. You also don't need knives, forks, spoons and plates to eat, but it makes your life much easier if you use them.

---

Now, let's do it! If you simply want to give up entirely and change majors, all you have to do is the following:

```
git pull -rebase origin master
(behold - the issue!)
git rebase --abort
(now you're free to change majors! you'll never use git or github again)
```

or, after seeing the description of the issue, navigate to the files, edit them manually to solve the issue and then
```
git mergetool
git rebase -continue
```

or, instead of using the CLI interface, fix the issue using either VS Code, GitHub Desktop, or even the issue handling thingy at the GitHub website!



