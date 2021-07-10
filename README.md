![CREATEmory Logo](./logo.png)
--
#### Lesson 1: *Intro To CREATEmory* 👋 <br/> Duration: *1 Hour* <br/> Topics: *CREATEmory, Github, Command-Line, HTML/CSS* <br/>

--
## Lesson Objectives
***After this lesson students will be able to:***

   * Explain the purpose and vision of CREATEmory
   * Use the basic tools necessary to build software (IDEs, Terminal, etc...)
   * Understand the basics of Github and Git
   * Understand the basics of the Command-Line
   * Create a simple webpage using HTML & CSS

----
## What is CREATEmory
CREATEmory is, above all, a **community of software engineers** who find it fun to work on **practical, creative applications**. It is a place to meet like-minded students and collaborate with them on **real-life projects**.

Next in order, CREATEmory is an organization that:
    
*  **Teaches software engineering skills** to Emory students through comprehensive, student-run courses (like this one!).
*  **Provides real project experience**, both from with Emory and outside, for students to apply their newfound skills.
*  **Manages the execution of projects** by organizing teams and training students on best Project Management practices.

#### During this course, you will learn how to properly work in a team of developers. Once ready, you will be able to work within real teams, on real projects.
<br/>

----

## Software Built For Building Software

#### Terminal:

We will go over the Terminal and the Command-Line later on in this lesson, but for now, **if you are using Windows, please download <a href="https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.1" target="_blank">Windows Powershell</a>** so it is easier to follow along with the instructor.

#### IDE:
Your IDE (Integrated Development Environment) is the code editor that you will use to write your code. For this course, **we suggest downloading <a href="https://code.visualstudio.com/download" target="_blank">Visual Studio Code</a> to use as your IDE**. However, if for whatever reason you don't lie VSC, <a href="https://atom.io/" target="_blank">Atom</a> or <a href="https://www.sublimetext.com/3" target="_blank">Sublime</a> are also solid options.

<img width="250" align="right" src="https://aprogrammerlife.com/images/pictuers/why_microsoft_word_is_the_best_ide_for_programming.jpg">

> For those of you who have already taken CS courses and are used to coding in Java, you might be tempted to use a Java-specific IDE like IntelliJ, but, because we will not be using Java, it would be better to use another option.


### Ultimately, which tools you use to build software are up to you. Pick whichever feels best. 

<br/>

----
## Terminal

Your Terminal is your Command-Line interface. Learning how to use it will drastically improve your efficiency while navigating through files, running programs, and executing many other tasks. **For now, we will just go over the basics so that you're ready to use Git and Github.**

> If you are using Windows, you will have to follow along with Windows Powershell. Most of the commands will be the same, but there are a few differences.

🔴 **Open Terminal**

- `⌘ (Command) + Space`, or use Spotlight
- "*Terminal"
- `Enter`

> You can customize the appearance of your Terminal by going to `Terminal > Preferences > Profiles`

#### Bash
Initially, your Terminal is set up to run the Bash scripting language. All you have to do is type in a command and press enter to run it.

🔴 **Try Out Some Common Bash Commands**

- `pwd` - will print the absolute path to the current working directory.
- `ls` - Lists the contents of the current directory. But it will only list the non-hidden files unless you add **Flags...**

#### Flags

Flags can be added to many Bash commands to modify them. They are denoted by a dash `-`. For example, if you wanted to list the contents of the current directory, you would add the `-a` flag to `ls` and type: `ls -a`

> A useful Flag that can be used on most commands is the `--help` flag,  which will print out additional information. Not that the help command requires two dashes `--`.

#### Navigating With the Command-Line

One command you will use very often is `cd`. `cd` stands for "Change Directory" and using it will do exactly that.

🔴 **Navigate Through Some Folders**

- `cd some_directory` *(Note that if you type `cd` and then click Tab, you can view your options and autofill)*
- `cd ..`
	- `..` refers to the parent folder, so using it will navigate you back to where you started. If you want to refer to the current folder, use `.`
- `cd`
	- If you use just use `cd` without specifying where to go, it will just take you to the home directory

🔴 **Try Some Other Very Common Commands**

- `mkdir directory_name` will create a new directory in the current folder
- `touch file_name` will create a new file in the current folder

### This is a very basic overview of the Command-Line. We recommend you spend some time practicing on your own. *For further Command-Line information and practice, <a href="https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory/blob/main/TERMINAL.md" target="_blank">please follow these instructions</a>. You will learn more commands and have access to extra assignments.*

<br/>

-----
## Github and Git
So far, you have been viewing this lesson through you web browser on Github.com. However, Github is not merely a place to store files. It is an incredibly useful tool that allows you to share code, work together on code, and maintain a history of your code. Github is just the online version of Git.

#### What is Git?

**Git is a version control too.** It allows you to **store and navigate a version history** of whatever project you are working on. Itn also allows you to move project **specific files from your "local" (or personal) computer to another internet-connected computer** which is acting as a central location for your code. This other computer is called a "remote repository."

All other computers that want to contribute to this specific project, will use the same remote repository (central computer), but send files from their own local computers.

#### Why should we use Git?

- In the old days, people would use FTP (File Transfer Protocol) to send their files to central computer
	- The issue:
		1. Two people (Person A, Person B) copy the same file from the remote repo at roughly the same time
		1. They both make changes
		1. Person A uploads their changes
		1. Person B uploads their changes, overwriting Person A's changes
- The next step was to create a locking mechanism
	- How it worked
		1. Person A would "check out" a file (like in a library)
		1. Person B would not be able to check out that file until it was checked back in
		1. Person A would make changes to the file and then check it back in
		1. Person B could now check out that file
	- The issue
		- Person B would have to wait for person A to finish with a file to start work on it
- The next step was tools like CVS and SVN
	- How it worked
		1. Both Person A and Person B could check out a file at the same time
		1. Person A modifies the file and checks it back in
		1. Person B modifies the file, tries to check it back in, but cannot
		1. Person B must re-check out the file that now includes the changes made by person A
		1. CVS/SVN will attempt to merge the changes together
		1. As long as the changes made by both Person A and Person B are on different lines, this will succeed
		1. Once the changes made by Person A have been merged with Person B's version of the file, Person B can now check in their file
	- The issue
		- If a person is not ready to check in a file, there is no way to keep track of the changes made to that file
		- If something goes wrong before checking the file back in, the user must, figure out what happened, go through an almost endless number of Undo commands in their text editor, or revert their file to version that is in the repository.  A lot of work could be lost
- Git functions just like CVS and SVN, but it adds a local repository
	- This allows a user to keep a log of their local changes before finally pushing everything back to the remote repository
	- The user can also travel "back in time" to previous states that have been saved locally, but not yet pushed to the remote repository.  This is great for when something goes wrong
	- The process:
		1. Add files whose changes you want to be logged
		1. Log the changes of the files that were added (called making a "commit")
		1. Once all commits have been made, and you're ready to send your changes to the remote repo
			1. "pull" any changes that have been made to the repo since you last synced your local repo with the remote repo
			1. "push" your changes to the remote repo.

##  Add an ssh key to your github account

- When you get tired of always entering your github password, you can use the ssh URL (as opposed to the https URL) when cloning a repo
- You'll need to also add what's called an ssh key to github https://help.github.com/articles/generating-an-ssh-key/
- Now you can use the ssh url when cloning instead of https

##  Create a repository in github

1. Go to https://github.com/
1. On the right click the green button that says "New Repository"
1. Give the repo a name and click Create

##  Clone that repository

1. Once you've created the repo, you'll be taken to repo page
1. In the "Quick setup" section, copy and paste the https url
1. Go to a suitable location in the terminal (let's do `~/dev/`) and type `git clone ` and paste the https url (e.g.`git clone https://github.com/mahuntington/asdfasdf.git`)
1. You may need to enter your github password

##  Stage Files

Once you've finished making changes for the moment, it's time to tell git which files need to have their changes logged

- `git add specific_file.txt` will log all changes to the file specific_file.text
- `git add .` will log the changes to all files in the current working directory
- `git add some_dir/` will log the changes to all files in the some_dir directory
- `git add -A` will add all files in the local repo that have been modified

To see the status of which files are in the process of being committed use `git status`

##  Commit Files

Log the files, and give the log a description (or "message") so you can easily remember what was done

- `git commit -m "changed the database structure to allow for an email address for each user"`
- check your commits with `git log`

##  Push files

Push your changes to the remote repository

- `git push origin master`
- origin is the nickname of the remote repo.  Master is the name of the branch (covered later), this is usually master when you start out.

##  Pull changes from remote repo

Pull any changes others made to the repo into your local version of the repo

- `git pull origin master`

##  Fork a repository

Open source software is popular because the source code for an open source application is available for viewing on the internet.  If you want to play around with the code of an open source app on github, you can simply fork the repo and make changes to it there.

1. Find the repo on github.com
1. In the upper right, click the `fork` button
1. Choose which user (or organization if you belong to any) should create the duplicated repo
1. Clone, add, commit, push as normal

##  Pull changes from original repo

Sometimes you want to get changes that have been made to the original repository

1. Add original remote repo with `git remote add upstream https://github.com/mahuntington/asdfasdf.git`
	- `upstream` is a conventional name, it can be anything, though
	- update the URL to that of the original repo NOT your fork
1. Pull with `git pull upstream master`

## Create an issue for the original repository

Sometimes you want to send messages to the maintainers of the original repository

1. Go to the original repo on github.com
1. Click on the "Issues" tab at the top
1. Click the green "New issue" button on the right
1. Enter a title and a comment
1. Click "Submit new issue"

##  Create a pull request to original repository

If you have made a change to your fork that you want to be integrated into the original repo, you'll have to ask the original repo owner to review and merge your changes into theirs.

1. Go to the original repo
1. Click the tab marked `Pull requests`
1. Click "New pull request"
1. Underneath "Compare changes" click "compare across forks"
1. For the "head fork" choose your fork.  Leave "base fork" as the original repo
1. Next to the "base fork" and "head fork" buttons are drop downs for which branch of your fork (compare) should be merged into which original repo branch (base).
1. Click "Create pull request"

##  Create a branch

- When working on a specific feature, it's generally a good idea to create a "branch"
- This is purely for organizational purposes
	- In general, the `master` branch is for finished features
	- If you are working on a feature, it's not complete, but you want to save those changes to the repo (perhaps it's the end of the day), you can use branches to keep your changes off the `master` branch
- To list all branches run `git branch`
- To create a new branch run `git branch newbranch`
- Switch to a branch using `git checkout foo`.  From now on, until you change branches again, all commits will be created on that branch

## Push a branch to the repo

- `git push origin newbranch` will push the currently active branch to the remote on a branch called "newbranch"
- in general, you should push a local branch to a branch on the remote repo with the same name

##  Merge a branch into another branch

Once you are finished with branch and want to merge it (usually back into master):

1. switch to the branch that you want to merge the new branch INTO (`git checkout master`)
1. merge the branch using `git merge newbranch`.  This will merge the `newbranch` branch into the currently active branch (usually `master`)
































