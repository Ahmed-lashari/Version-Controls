# Status Codes: Short status flags are:

#### ?? or U - Untracked files
#### A - Files added to stage
#### M - Modified files
#### D - Deleted files

### Here in this file we will create 2 branches and them will merge both of them into the main or master branch (main in our case)

## 1. Checking current Branchs

```bash
git branch
```

Output:
```bash
* main
```
## 2. Creating a New Branch

```bash
git branch custom-merging-branch
git branch
git switch custom-merging-branch
git branch
```

Output:
```bash
ahmedlashari@192 Verrsion-Controls % git branch custom-merging-branch

ahmedlashari@192 Verrsion-Controls % git branch
  custom-merging-branch
* main

ahmedlashari@192 Verrsion-Controls % git switch custom-merging-branch
Switched to branch 'custom-merging-branch'

ahmedlashari@192 Verrsion-Controls % git branch
* custom-merging-branch
  main
```

## 3. Pushing into the repository

After working (making changes) in the newly-created-branch, we will commit and push it to the feature branch to github, like this:

```bash
git add .                                 # add all files
git comit -m "pushing feature branch"     # or the branch name here
git push origin custom-merging-branch     # code will be pushed to GITHUB
```

## 4. Merging into main Branch

After Analyzing and testing the changes from new branch, the changes will be merged into the main branch from the GitHub Repository UI by clicking hte *"Compare and Pull"* button or in the terminal like this:

Compare the changes:
```bash
git diff main

# or see the summary 

git log main..feature/update-home-ui --oneline
```

Switch to main branch after analyzing chnages:
```bash
git checkout main
```

Pull the Latest main from GitHub (just in case to remain updated) 

```bash
# recommended but not needed
git pull origin main
```
Merge Feature Branch into main Locally
```bash
git merge feature/update-home-ui
```

### ✅ This will merge the changes from the feature branch into main.

#### ***Just for a Safe Side:***
Push the Updated main to GitHub

```bash
git push origin main
```

# ✅ Optional Cleanup
```bash
git branch -d custom-merging-branch          # Delete local branch

git push origin --delete custom-merging-branch   # Delete remote branch
```


# In Our Case the Folder Flow was a bit unadjusted, so doing another merge request from the custom branch and then pulling into main branch. (Not Needed for You)


After adjusting the file in its folder:
```bash
git add .

git commit -m "branch-merging file adjusted into the folder"
```

