# my-first-PR
First pull request for beginners - practice open-source project!

## INSTRUCTIONS
### Fork & Clone
- Press the fork button on Github
- Set up a local version by cloning the repo

### Add upstream
The local repository has a remote called `origin`. This is the remote version of your personal fork of the original project hosted on Github. You need to add a second remote, call it `upstream` so that you can pull changes from it in the future.

- Do this by navigating back to the original repo and get the "SSH clone URL" 
- After changing into the local directory in your terminal, add a new upstream:
```
$ git remote add upstream git@github.com:rgomezp/my-first-PR.git
```

### Branch!
It is customary to create a new branch for every new feature/chunk of code. 
- Make sure you're on the `master` branch
- Create a new branch. Name it something related to the new change you are adding -- in this case `add-name` might be a good option.
```
$ git checkout -b add-name
```

### Add your name
Make the changes you want. In this case, add your name to the list along with a link to your LinkedIn or Github page.

### Push the new branch
Before creating a PR (pull-request), you need to push the new branch to your personal remote. Use the `-u` flag to make sure that the current branch is tracking the remote one. You can simply omit the flag and branch name in the future.
```
git push -u origin add-name
```

### Create the PR
Head back to the repo in your browser and click the button that creates a new PR. On the next page, make sure the "base fork" and "base" point to the original repo + branch, respectively. The "head fork" should point to your own fork of the repo and the "compare" should point to your new branch.

####
Hit "Create pull request" and you're done! At this point, maintainers will review your work and if satisfactory, merge it.
