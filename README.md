# git_practise
This is just a simple Project to help FTC Teams to see how git works, including a few exercices

In this exercise we will do the following:

## Firts Things first:

You have to create a your own ```git``` Account

Visit the link for simple examples and how to setup your git [https://rogerdudler.github.io/git-guide/]

Also Learn git in 10 minutes: [https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/]

1. Clone the Project
2. Make some changes, commit and push the Changes.

### Exercise 1: Clone the Project

1. Install a ```git``` client
2. On your PC create a directory where you want to clone the Project
3. Run the following command (Assuming you use a simple git terminal type Client) ```git clone https://github.com/mtbbiker/git_practise.git```
4. If you make changes and you would like ```push``` your changes to the original project, you will have to request a ```Pull Request``` more on that later

### Exercise 2: Fork the Project

This you can do on the ```github``` web page. This will create a ```copy``` of the project in your namespace
1. Search for the ```repository``` that you want to fork if you don't own the repository
2. Click on the ```Fork``` button (to the Top of the web page, next to the ```Unwatch``` and ```Star``` button)

### Exercise 3: Create a new Branch

Branching is normaly used for maintaining and Testing code, then once it passes all test it will be merge back to the Master. The master will then typicaly used for Releases.
1. ```Click``` on the ```Branch:master``` button. Use the Find or create a new branch
2. On your PC you will have to pull the Branch. 

```git pull```
And a Typical Result:
```
$ * [new branch]      development -> origin/development

```
3. To change to this new Branch for further work execute the following command:
```git checkout -b development```

4. Change some code.
5. View the status of your changes: ```git status```
```
eugene@atlanta:~/Private/FTC/git_practise$ git status
On branch development
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
6. Add your change ```git add README.md```
7. Commit your code: ```git commit -m 'My new change'
8. Push your changes: ```git push```  

If you have not set the Upstream you will get a message like
```
eugene@atlanta:~/Private/FTC/git_practise$ git push
fatal: The current branch development has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin development
```
9. Set the upstream Branch: ```git push --set-upstream origin development```, Then push again

### Exercise 4: Merge your Branch to the master

