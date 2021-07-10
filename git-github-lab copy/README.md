![GA logo](https://camo.githubusercontent.com/6ce15b81c1f06d716d753a61f5db22375fa684da/68747470733a2f2f67612d646173682e73332e616d617a6f6e6177732e636f6d2f70726f64756374696f6e2f6173736574732f6c6f676f2d39663838616536633963333837313639306533333238306663663535376633332e706e67)

## SEI

# Github, HTML and CSS practice (Resume Page)

---
Title: Github, HTML and CSS practice (Resume Page)<br>
Type: Lab/Homework<br>
Creators: Various instructors <br>
Competencies: Github, command line git, HTML, CSS<br>
Prerequisites: Github, git, HTML, CSS

---

## Part 1 - Github

### Read all the instructions below before you do anything.  With every lab/homework/project/activity/exercise we give you, ***always*** read through all the instructions before you do start.

0. **Do not fork this repository.**

1. If you cloned this repository, `cd` into the folder that was created by the clone and then skip the rest of this step.  If you did *_not_* clone this repository, create a directory called `git-github-lab` in your directory for today and `cd` into it.  Initialize a git repo. (`git init`). **Do not run `git init` if you are already in a repository that you cloned**. You can check if you're already in a repo by running `git status`.  If it says `fatal: Not a git repository (or any of the parent directories): .git`, then you are **not in a repo** and it is safe to run git init.  If it says ANYTHING ELSE, then DO **NOT** run `git init`.  You do not ever want to run git init inside of an existing repo.  **No git repos inside of git repos!!!**

2. In the top level of your repository, create a file `github-lab-answers.md` and answer the questions below. Commit your work at each point when directed.

2. Look at the questions below and answer them as you complete this tutorial: <https://try.github.io>

3. This tutorial is also great for learning git: http://gitimmersion.com/ It's fairly long, but don't feel like you need to pick it all up in one sitting—you can come back to it.

---

### Answer the following questions

1. What command do you use to setup a git repository inside of your folder?<br>
1. What command do you use to ask git to start tracking a file?<br>
1. What command do you use to ask git to move your file from the staging area to the repository?<br>

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 1 - The 1st set of GIT homework answers are complete".
<hr>

1. What command do you use to pull any changes from the master repository into your local repository?<br>
1. What command do you use to unstage a file?<br>
1. What command do you use to change your files back to how they were after a commit?<br>
1. Why is it important to use `--` when changing files back to a previous state?<br>
1. Why might you want to reset your files back to a previous commit?<br>

<hr>
&#x1F534; ** Commit your work.** <br>
The commit message should read: <br>
"Commit 2 - The 2nd set of GIT homework answers are complete".
<hr>

1. What command do you use to create a branch?<br>
1. What command do you use to use a different branch?<br>
1. Why would you want to use a branch other than the default `master`?<br>

<hr>
&#x1F534; ** Commit your work.** <br>
The commit message should read: <br>
"Commit 3 - The 3rd set of GIT homework answers are complete".
<hr>

1. Give an example for when you would use `git merge` and give an example for when it would be better to submit a pull request to have your branch merged<br>
1. What command do you use to send all of the work that you've done locally to your remote repository?<br>

<hr>
&#x1F534; ** Commit your work.** <br>
The commit message should read: <br>
"Commit 4 - The 4th set of GIT homework answers are complete".
<hr>

## Part 2 - HTML Video

Watch [this video on HTML](https://www.youtube.com/watch?v=DxhXFpsN5I4&index=1&list=PLdnONIhPScST0Vy4LrIZiYKpFNoxgyH7J).

## Part 3 - Fake Resume Site

#### Setup your folder and files

1. Inside the `github-lab` directory, create a new directory called `resume_page`.
1. Change directories to `resume_page`. Create two files: `index.html` and `style.css`.<br>
1. Using Sublime, open your files and add the HTML boilerplate code.<br>
1. Create a heading level-one tag with your name.<br>
1. Open the `index.html` in your browser to confirm that everything is set up properly.
Reminder: To open your file with your browser, from the command line, type `open index.html`

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 5 - index.html file is setup".
<hr>

#### Add some content to your site

1. Insert a professional image of yourself or someone else ('img' tag); it should be placed right after your 'h1' tags<br>
1. Insert an unordered list of your last three positions ('ul' tag)<br>
1. Create links to your (or someone's) LinkedIn and Facebook/Twitter pages ('a' tag)<br>1. Use level-three heading tags to create headings before your positions and before your links<br>

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 6 -  Added initial content for resume site".
<hr>


#### Add some style to your site

1. Center your "h1" tag<br>
1. Change the font of your "h1" tag<br>
1. Change the color of the font of your "h3" tag text<br>
1. Add some space on the body of your application to make your site look more appealing.<br>

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 7 -  Added initial styling for resume site".
<hr>


#### Add some navigation to your site

1. Create a nav bar with the links to your LinkedIn, Twitter (whichever links you had created earlier); Remove the links section that you had created earlier in the homework.
1. In the nav bar, also create a link to the 'index.html' page (maybe give it a name of `Home Page` in the bar), and a link to a file called "projects.html" (maybe call this `Projects` in the bar) <br>
1. Create another html file in this folder called 'projects.html'<br>
1. Copy the contents of the nav bar and information from the 'head' tag of your `index.html` file and paste it into your `projects.html` file<br>
1. Inside `projects.html`, create a level-two heading and add the text `Projects`<br>
1. Check to make sure that your links work! When you click on "Projects" in your nav bar, does it open the `projects.html` document?<br>
1. In 'projects.html', add your three most recent projects (or just make some up). To do this simply, you can use an ordered list. If you're up for a little more of a challenge, create three columns: each column should contain the title and a description of your three most recent, successful projects<br>

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 8 -  Added project.html page and content".
<hr>


## Part 4 - Loops
#### Stay Fresh! Looping with Javascript

* In the `github-lab` folder, create a directory called `loop-questions`.  In `loop-questions` directory, create our usual folder structure with the `index.html` that has the `app.js` linked up in a `<script>` tag. After each question, test your code by reloading the browser and checking the console.
1. Create a loop that logs the numbers from 0-99, (ascending)
2. Create a loop that logs the numbers from 99-0 (descending)
3. Create a loop that logs the numbers from 298-1, **counting** down by 3 (the code in the loop should run 99 times)
4. Create a loop that logs the **EVEN** numbers from 0-98 (ascending)
5. Create a loop that logs the **ODD** numbers from 98-0 (descending)
6. Create a loop that logs the numbers from 49-72 (ascending)
7. Create a loop that logs the numbers from 81-26 (descending)
8. Create a loop that logs the numbers from 1-91 **that are multiples of 3** (ascending)

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 9 - Created loops.js file".
<hr>


## Hungry for more?

- Check out this [tutorial](http://gitreal.codeschool.com/?utm_source=github&utm_medium=codeschool_option&utm_campaign=trygit) that includes videos about using git and some challenges for you to tackle.

##### More for your site:
* Insert a video of your work or your favorite YouTube video ('iframe' tag)<br>
* Add a level-three heading above your video with a title for the section<br>
* Insert a table with your contact info (`table` tag)<br>
* Add a level-three heading above your contact info with a title for the section<br>

* Give the image a 1px black border<br>
* Give the body of the page a thicker border than the picture but only on the top and bottom of the page<br>
* Using HTML, insert a short blurb or biography with "p" tags<br>
* Using HTML, insert a short description above your "p" tag; use an "h3" tag<br>
* Make your name uppercase <strong>using CSS</strong><br>

* Insert another image of you, or an image of one of your projects, but make it round<br>
* Insert a button on both pages that links to opening an email to your email address<br>
* Style your navigation bar<br>

<hr>
&#x1F534; **Commit your work.** <br>
The commit message should read: <br>
"Commit 10 -  Worked on Hungry for More".
<hr>


## Conclusion

 1. Inside the `git-github-lab` directory, you should now have a file called `github-lab-answers.md`, a directory called `loop-questions`, and a directory called `resume_page` which contains `index.html`, `projects.html`, and `style.css`.

 2. You should have been adding and committing along the way, but please type `git status` one last time to make sure that everything is committed. If it's not, please commit.



