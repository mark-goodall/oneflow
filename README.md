# oneflow
Helpful commands to help with git oneflow, based on this [blogpost](http://endoflineblog.com/oneflow-a-git-branching-model-and-workflow) in a response to gitflow.

The tooling in this repo are based on feature branch scenario 3 (rebase + no ff), with the additional feature of `bugfix` branches. While identical to feature branches, they've basically got some additional syntactic sugar to easily identify the bug id and auto link and resolve it when pushing to origin. A small variation has been added for the feature branches. Instead of merging to master, they will follow the same flow and open the git repo url so you can start a pull request instead.

Add these to a folder that is included in your path variable. You can then call them as follows:

```
 > git bugfix 
 > git feature
 > git finish
 > git hotfix
 > git latest
 > git latest-tag
 > git open
 > git release
```
You can pass `--h` for a short readme, as follows:

```
> git bugfix --h
```

And yes, I do realize it's ironic he makes a note in his blogpost that he doesn't like tooling for flows like these.. :-)
