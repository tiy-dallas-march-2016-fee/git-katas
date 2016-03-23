# Kata 1: Basic Git Checkin

This kata is designed to practice creating a repo on GitHub and pushing files to that repo.

## Long Explanatory Version

The first time you do this kata, use this version. When you think you understand it well, use the short version below.

* Step 1: Go to [GitHub](https://github.com) and login if you are not currently logged in.
* Step 2: Create a new repository. Name it anything you like, though I would stick with alphanumeric characters, dash, and underline.
* Step 3: Go in your terminal to where you keep your code on your laptop. As an example, my code goes here: `/Users/ericsowell/Dev`.
* Step 4: Clone the repo you created in step 2. Issue the command `git clone https://github.com/<your-user-name>/<repo-name>.git`.
You will probably see a message that looks something like this:
```
Cloning into 'katapractice1'...
warning: You appear to have cloned an empty repository.
Checking connectivity... done.
```
The warning isn't bad. You are in fact cloning an empty repository.
* Step 5: Use the `ls` command. Note that you should have a folder with the same name as the repository you created in step 2.
* Step 6: Change into that directory so you are at the root folder of that Git repository. If you issue a `ls -a` command, you should see a `.git` folder. There should be no files.
* Step 7: Create an html file named `page.html`. Either do that by issuing `touch page.html` in the console or create the file with your editor.
* Step 8: Create a simple web page with a paragraph that says `Hello Git kata!`. If you want to open the directory in Atom that you are in, issue the `atom .` command.
* Step 9: Back to the terminal. Issue the `git status` command. You will see something like the following. This means that Git noticed you have changes (you added a file) but is currently choosing to ignore it/not track it.
```
Erics-MBP-2:foo ericsowell$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	page.html

nothing added to commit but untracked files present (use "git add" to track)
```
* Step 10: Now we will make git track the changes. Issue this command in the terminal: `git add page.html`.
* Step 11: Issue the `git status` command. You should see the following. Git is now tracking your changes, but they aren't saved into the repository.
```
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   page.html
```
* Step 12: Issue the `git commit -m "committing new page"`. The change is now in your *local* repo but not up on GitHub, which is your *remote* repo.
* Step 13: Go to GitHub. Refresh your repo page. You should *not* see your file yet because you have not pushed it yet.
* Step 14: Issue the `git status` command. You should see something like this:
```
On branch master
nothing to commit, working directory clean
```
* Step 15: Issue the command `git push`. Depending on how you have Git configured, you may see more or less text than this. But you should at least see something very similar to this, possibly toward the bottom:
```
Counting objects: 3, done.
Writing objects: 100% (3/3), 249 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/Mallioch/steak.git
 * [new branch]      master -> master
```
* Step 16: Go to GitHub. Refresh your repo page. You *should* see your file.
* Step 17: Congratulate yourself! You have checked your code in to your local repo and up on GitHub.

## Short Version

* Step 1: Go to [GitHub](https://github.com) and login if you are not currently logged in.
* Step 2: Create a new repository.
* Step 3: Go in your terminal to where you keep your code on your laptop.
* Step 4: Clone the repo you created in step 2.
* Step 5: Change into that directory so you are at the root folder of that Git repository.
* Step 6: Create an html file named `page.html`.
* Step 7: Create a simple web page with a paragraph that says `Hello Git kata!`
* Step 8: Now we will make git track the changes. Issue this command in the terminal: `git add page.html`.
* Step 9: Issue the `git commit -m "committing new page"`. The change is now committed locally.
* Step 10: Issue the command `git push`.
* Step 11: Go to GitHub. Refresh your repo page. You *should* see your file.
* Step 12: Congratulate yourself! You have checked your code in to your local repo and up on GitHub.
