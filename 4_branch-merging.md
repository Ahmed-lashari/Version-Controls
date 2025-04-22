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