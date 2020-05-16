# RUHacks 2020 How to Collaborate with GitHub	

The app page can be viewed here: [http://maihameed.me/ruhacks20](http://maihameed.me/ruhacks20)	

## Contributing an avatar	

1. Click the `contributors.json` file to open it up
2. Click on the edit button, it looks like a pencil
3. Add your GitHub username to the list, make sure it's somewhere above `"MaiHameed"`
4. (optional) Add a title for your commit
5. Click the `Propose file change` button, it will automatically take you to the 
   "Open a pull request" page
6.  Ensure that the head repository is your forked repository, it should be
   `<your-username>/ruhacks20`, and the base repository is `MaiHameed/ruhacks20`
   (it should be by default).
7. Click the `Create pull request` button.

Congratulations! You've opened a pull request! Find and comment on another person's 
pull request, and wait for me (Mai) to merge your changes. Once merged, you can
revisit [http://maihameed.me/ruhacks20](http://maihameed.me/ruhacks20) to view your
newly added avatar and hyperlink!

## Contributing using the CLI

Check out the [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

1. Make sure you have Git installed, test it by running the following `git verison`,
   you should get an output similar to:
```
git version 2.24.1 (Apple Git-126)
```
2. Fork the `MaiHameed/ruhacks20` repository, it'll create a copy of the repository
   on your profile with the same name
3. Visit your fork, and click the `clone or download` button, and copy the URL
   for HTTPS cloning
4. In your terminal run the following command to clone your repo:
```
git clone <url>
```
5. Navigate to the newly cloned `ruhacks20` directory:
```
cd ruhacks20
``` 
6. (optional) Create a new branch to make your changes in. Typically, best practice
   calls for your branch name to have a consice title that
   showcases what the branch is doing. For example `delete-name`. Run the following
   command to create a new branch and switch to it:
```
git checkout -b <your-branch-name>
```
1. Delete your name from the `contributors.json` file (you can use vim or any text
   editor or IDE)
2. In your terminal, run the following command to stage your change for a commit:
```
git add contributors.json
```
8. Run the following command to commit your change with a short commit message:
```
git commit -m "your commit message"
```
9. (optional) If you made your changes in a separate branch, run the following to
    merge your changes to your `master` branch:
```
git checkout master
git merge <your-branch-name>
```
10. Run the following command to push your master branch to your remote repository
    (your `<your-username>/ruhacks20` repository)
11. Revisit your repository on GitHub to view your latest commit
12. Navigate to the `Pull requests` tab
13. Click on `New pull request`
14. Create a pull request from your master branch to mine
15. Look for your pull request on the `MaiHameed/ruhacks20` repository to ensure
    that it went through

Congratulations! you used the Git CLI to open a pull request!

## Serving locally	

You can clone this repo and run it locally on your machine. To do so you'll need
to install `node.js` and `npm` and run the following command in your terminal:

```	
npx serve	
```