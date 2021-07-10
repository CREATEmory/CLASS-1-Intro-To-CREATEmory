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

### [Here is the link](https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory/blob/main/GIT-LAB.md) to the Lab that you should complete after this lesson

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

### What is Git?

**Git is a version control too.** It allows you to **store and navigate a version history** of whatever project you are working on. Itn also allows you to move project **specific files from your "local" (or personal) computer to another internet-connected computer** which is acting as a central location for your code. This other computer is called a "remote repository."

All other computers that want to contribute to this specific project, will use the same remote repository (central computer), but send files from their own local computers.

![Git Image](https://www.nobledesktop.com/image/blog/git-branches-merge.png)

### Why should we use Git?

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

##### Git functions just like CVS and SVN, but it adds a local repository

- This allows a user to keep a log of their local changes before finally pushing everything back to the remote repository
- The user can also travel "back in time" to previous states that have been saved locally, but not yet pushed to the remote repository.  This is great for when something goes wrong

![Local Servers](https://www.edureka.co/blog/wp-content/uploads/2016/11/Distributed-Version-Control-System-Workflow-What-Is-Git-Edureka.png)

### The "Add, Commit, Push" process:

1. Add files whose changes you want to be logged
1. Log the changes of the files that were added (called making a "commit")
1. Once all commits have been made, and you're ready to send your changes to the remote repo
	1. "pull" any changes that have been made to the repo since you last synced your local repo with the remote repo
	1. "push" your changes to the remote repo.

	
## How to use Git and Github

### 1. Create An Account On Github 🔴

- **[Link To Github](https://github.com/)**

### 2. Go to a repository on github 🔴

1. Go to the [repository for this lesson](https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory) (Hint, you should already be there)


1. In the top right corner, click the button that says "Fork" to create a copy of this repository on your own Github account.

> This is usually how open source software works. The source code for many open source applications is available for viewing on Github. If you want to play around with the code of an open source app on github, you can simply fork the repo and make changes to it there.

### 3. Clone that repository 🔴

<img src="https://docs.github.com/assets/images/help/repository/code-button.png" align="right" width="350" margin="10" />

1. Click the big green "Code" button and copy the url


1. Go to a suitable location in the terminal (probably use the folder created for this class) and type `git clone ` and paste the https url (e.g.`git clone https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory.git`)

1. You may need to enter your github password

> If you would like to avoid entering your password everytime, you can add an ssh key to your github account. You'll need to also add what's called an ssh key to github. [Do that by following these instructions](https://help.github.com/articles/generating-an-ssh-key/). Then you can use the ssh URL (as opposed to the https URL) when cloning a repo.

> Alternatively, you can [follow the instructions in this guide](https://gist.github.com/jonjack/bf295d4170edeb00e96fb158f9b1ba3c) and add your Github credentials to your Terminal Keychain.

###  Adding and Committing Files

Now that you have the files on your computer, **you can make changes to them** however you want. But after you make a significant change, you ought to add and commit it to track those changes.

#### Adding Files  🔴

- `git add specific_file.txt` will log all changes to the file specific_file.text
- `git add .` will log the changes to all files in the current working directory
- `git add some_dir/` will log the changes to all files in the some_dir directory
- `git add -A` will add all files in the local repo that have been modified

To see the status of which files are in the process of being committed use `git status`

- **For the most part, you should just use `Add .` unless you have a specific reason otherwise.**

####  Committing Files  🔴

Log the files, and give the log a description (or "message") so you can easily remember what was done

- `git commit -m "changed the database structure to allow for an email address for each user"`
- check your commits with `git log`

###  Push files  🔴

Push your changes to the remote repository. This means that the Github version will be updated.

- `git push origin main`
- origin is the nickname of the remote repo.  Main is the name of the branch (covered later), this is usually called "main" when you start out.

###  Pull changes from remote repo

If you were working with others, and they made changes to the repo, you could pull those changes into your local version of the repo with:

- `git pull origin main`

### There is much more to learn about Github, but this is all we will cover for now. If you want to learn more about Pull Requests, Branchs, Merging, etc. you can [read through this](https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory/blob/main/GIT.md) for now.

<br/>

----

## HTML and CSS: The Basics

#### There are [many](https://learn.shayhowe.com/html-css/building-your-first-web-page/), [many](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics), [many](https://html.com/) resources already made for learning HTML/CSS. If you are totally unfamiliar, it would be a good idea to review some of them, as we only have time to go over the bare minimum.


### What is HTML?
HTML stands for "HyperText Markup Language." Think of it as the building blocks of a website. In general, every element you see on any website is simply one, or a collection of HTML elements.

For example, this text look like this in HTML: 
`<p>For example, this text look like this in HTML: <p/>`

<img src="https://michaelvbachmannbloghome.files.wordpress.com/2020/07/elements.jpg" align="right" size="200"><img/>

As you can see, it is wrapped with a `<p>` tag to indicate that it is a  paragraph. 

There are many many HTML tags to learn, and all of them do different things. We will go over them a bit, but it's best to learn as you go.

The photo on the right shows how you might think of laying out a simple webpage in terms of html.

> The code for that photo looks like this:
> `<img src="https://michaelvbachmannbloghome.files.wordpress.com/2020/07/elements.jpg" align="right" size="200"><img/>`


### What is CSS?

If every website is built up of the same basic HTML Elements, then why do they all look so different?

This is where CSS (Cascading Style Sheets). CSS is a language that allows you to edit the appearance of HTML elements. 

For example, if I wanted to make the `<p>` from before blue, 50px in size, and change the font, I would use this CSS code:
```
p {
	 font-family: 'Times New Roman';
    color: blue;
    font-size: 50px;
}
```

**CSS is an art, and it can gert very complex. We cannot cover everything in this lesson. But you will use it very often, so it is good to learn on your own time.** 

### How will we use HTML?
At first, we will use HTML in it's most basic form. Let's make a basic HTML page with some styles.

🔴 **Create a basic HTML/CSS page**

1. Create a new file in this folder called `index.html`

	> Hint: use the `touch` command on yout Terminal

2. Open the file in your browser with the command `open index.html`. For now it will be a blank white screen.

3. Open the command in your IDE (just use `code index.html` if you are using VSC)

3. Then we will add the "HTML Boilerplate". This is just a template of HTML elements that will be necessary on every HTML page for it to be interpreted properly. **Copy and paste this into your `index.html` file:**


```
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title></title>
</head>
<body>
  
</body>
</html>
```
> Note, nothing will show up on your browser. This is because these elements are either unstyled containers like `<body>` or they are used for non-visual aspects of a website

#### 🔴 Add some elements to your page

- Between the two `<body>` tags, you can now add whatever you want. Note: elements must have both an opening tag (`<element>`) and a closing tag (`<element/>`) with the content going in between the two.
	- `<p></p>` for a paragraph
	- `<h1><h1/>` for a header 1 (you can also use 2-6)
	- `<img src="url_to_image" ></>` for an image (note that you can add "attributes" to HTML elements like the `src=""` attribute on this `<img>` tag)
	- `<div><div/>` for a general container element
	- `<a href="url_to_go_to" ></>` for a link
	- etc...


### How to add CSS?

I'm sure your page looks a bit dull right now. Let's add some CSS to style it.

#### 🔴 Link CSS to your HTML page

1. Create a file to type your CSS in called `styles.css`

2. Open that file in your IDE

3. In your HTML file, you will have to link your CSS file. To do this, you will add a `<link>` element in the `<head>` of your HTML page with the path to `styles.css`. Like this:

```
<head>
  <meta charset="utf-8">
  <title></title>
  <link rel="stylesheet" href="styles.css">
</head>
```
#### 🔴 Style your HTML page with CSS

1. The most basic way of styling an HTML element in CSS is by refering to the name of the element. For example, to make all of the `<p>` elements on my page red, I would type `p { color: red }` in my CSS file. **However, this will apply that style to *every* `<p>` tag on my page.**

2. To style only specific elements, you can add IDs or Classnames to those elements. You do this by adding an `id` or a `class` attribute to an element. For example, let's say I have two different `<p>` elements, and I want to make one blue and one red.
	- First, I would add class names to those elements like this:
		- `<p class="red-text" >` and `<p class="blue-text" >`
	- Then, in my CSS file, I could reference them using `.classname`. For example:
		- `.red-text { color: red }` and `.blue-text { color: blue }`  

3. Add some styles to your html page. [Here is a good article](https://codeburst.io/how-to-style-your-website-with-css-e72e7046fda5) that goes over the CSS basics in more detail.

<br/>

---

## End Of Class

### ***Thank you all for coming.***

### Please fill out this form to give us feedback and record your attendance. **CREATE/ADD FORM TO THIS!!!**

### You are free to work on whatever you want. But we will have this room for a couple more hours, so please feel free to stay and work with others.

### For further practice, we reccomend that you [complete this lab](https://github.com/CREATEmory/CLASS-1-Intro-To-CREATEmory/blob/main/GIT-LAB.md) by next week.




