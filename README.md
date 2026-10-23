# Requirements

Python 3.13.x or 3.14.x

## Start up the DSA2101 environment

1. Create a new virtual environment
```
# Windows
py -m venv venv-dsa2101

# MacOS
python3 -m venv venv-dsa2101
```

2. Activate the virtual environment 
```
# Windows
venv-dsa2101\Scripts\activate

# MacOS
source venv-dsa2101/bin/activate
```

3. Install the packages
```
python -m pip install --upgrade pip

# Check if installed correctly
python --version
python -m pip list
```

4. Download the prerequsites pinned in telegram.

## Cloning the repository from github

1. Open github desktop
1. On the top left, click "Add" then "Clone repository"
1. Choose an empty folder to initialise your repository.

# Basics of git

A commit in git is used when we want to make changes to the codebase.

## Adding and commiting

`git add` adds code to commit. This does not actually commit but just prepares it (Staging). 
`git commit` commits the code locally. 

- CLI

```
git add * # Stages everything that was changed in your codebase to be commit
git add main.ipynb # Stages only main.ipynb

git commit -m "This is a commit" # Commits the staged code locally with the message "This is a commit" 

```

- GUI (For both adding and commiting)
1. On the left sidebar, click the source control icon.
1. Type in a commit message and click Commit. If possible, your commit message should be about what you added in this commit.
1. A pop up sometimes will appear, click "Yes".
[![Add and commit](README-img/Adding%20and%20commiting.png)]


# Git workflow

This is a basic guide on how our group will be using git to contribute to the codebase

We will use git branches to make sure that each duo will write code in isolation on their respective parts. Think git branches as different versions of our code that can exist at the same time.

### Initialise the branch for your duo (Only one time)

Creating a branch called duo-1
```
git switch -c "duo-1"

```
Switching to branch duo-1
```
git switch duo-1
```
You will be working **only** on the branch you and your partner created. 

### Add and commit to this branch

Refer to the segment [here](#add-and-commit-to-this-branch).

### Push your code to github

Remember that commiting your code is only local. You have to push to github so everyone in the project team can see it.

**CLI**
This code pushes to github on the branch duo-1.
```
git push origin duo-1
```

**GUI**

On github desktop, 

