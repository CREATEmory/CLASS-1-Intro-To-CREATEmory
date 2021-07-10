###  Create a pull request to original repository

If you have made a change to your fork that you want to be integrated into the original repo, you'll have to ask the original repo owner to review and merge your changes into theirs.

1. Go to the original repo
1. Click the tab marked `Pull requests`
1. Click "New pull request"
1. Underneath "Compare changes" click "compare across forks"
1. For the "head fork" choose your fork.  Leave "base fork" as the original repo
1. Next to the "base fork" and "head fork" buttons are drop downs for which branch of your fork (compare) should be merged into which original repo branch (base).
1. Click "Create pull request"


###  Create a branch

- When working on a specific feature, it's generally a good idea to create a "branch"
- This is purely for organizational purposes
	- In general, the `main` branch is for finished features
	- If you are working on a feature, it's not complete, but you want to save those changes to the repo (perhaps it's the end of the day), you can use branches to keep your changes off the `main` branch
- To list all branches run `git branch`
- To create a new branch run `git branch newbranch`
- Switch to a branch using `git checkout foo`.  From now on, until you change branches again, all commits will be created on that branch

### Push a branch to the repo

- `git push origin newbranch` will push the currently active branch to the remote on a branch called "newbranch"
- in general, you should push a local branch to a branch on the remote repo with the same name

###  Merge a branch into another branch

Once you are finished with branch and want to merge it (usually back into main):

1. switch to the branch that you want to merge the new branch INTO (`git checkout main`)
1. merge the branch using `git merge newbranch`.  This will merge the `newbranch` branch into the currently active branch (usually `main`)