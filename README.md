Welcome to my Git Tutorial within git!
======================================

Hello and welcome.

This tutorial is to help people
get more acquainted with the versioning tool known as `git`.

**This tutorial is a work-in-progress.
It is not yet a finished product ready to teach people git!**

There are lots of git tutorials out there,
but what makes this one different is that
the whole tutorial is a git repository
that you learn about git by navigating through.

This file, `README.md`, is a file in the repository.
We'll begin here.

First, Make sure you have `git` on your computer.  Go to
[getting git](/Getting git.md) if you need help.


Cloning the Repository
----------------------

Once you have `git` installed,
the first thing you'll want to do
is get a copy of the responitory onto your computer
so you can explore it and go through the tutorial.
This is called cloning the respository,
and it is done with the `git clone` command.

To clone the repository,
navigate to a directory where you'd like to put the code,
go to your Command Line and type this at your keyboard:

    git clone https://github.com/ryanfmurphy/git-tutorial-in-git.git


By the way, I just made a new branch
------------------------------------
I wonder what will happen when I commit and push to GitHub?
Will GitHub get this branch too?

    $ git commit -a
      <type in commit message and save and quit>
    $ git push

The commit went through fine,
but aha, when I did push this happened:

    fatal: The current branch new_branch has no upstream branch.
    To push the current branch and set the remote as upstream, use

    git push --set-upstream origin new_branch

So git isn't expecting me to push this branch to the remote
unless I explicitly configure it.
I'll try the command they recommend.

    $ git push --set-upstream origin new_branch

    Counting objects: 9, done.
    Delta compression using up to 8 threads.
    Compressing objects: 100% (9/9), done.
    Writing objects: 100% (9/9), 1.40 KiB | 0 bytes/s, done.
    Total 9 (delta 3), reused 0 (delta 0)
    To git@github.com:ryanfmurphy/git-tutorial-in-git.git
     * [new branch]      new_branch -> new_branch
    Branch new_branch set up to track remote branch new_branch from origin.

Cool, it worked!  Now when I go to GitHub I see
a notification that they got the new branch:

![](/images/new-branch.png)

...and when I go down to "Branch: master" and click
I get a menu of all the branches to choose from:

![](/images/new-branch-2.png)


