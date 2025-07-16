# 🚀 **Git and Github**
- install git in laptop other than C derive
- then open terminal and config by followiing code  
    - git config --global user.name ""
    - git config --global user.email ""
- Add github to your project
    - git clone paste link withot ""
    - git status
    - git pull origin main  
- Add project to the github
    - git init    ## to incorporate git in folder
    - Remove-Item -Recurse -Force .git #remove git
    - create repositor in github with same name of your projec and without rmd file
    - git add .
    - git commit -m "first commit"
    - git remote add origin repositor link #connect
    - git branch
    - git remote --v
    - git push -u origin main    #here -u represent upstream means it always adds changes automatically in origin/main branch with 
    - git push command  #use onward
---

## 🔁 GitHub Access Types – Short Guide


## 1. Fork → Clone → Change → Push

- ✅ Changes go to **their GitHub fork**
- ❌ Your repo is not affected
- ✅ They can open a **pull request** to suggest changes


## 2. Just Clone (No Fork)

- ✅ Gets a **local copy** of your code
- ❌ Cannot push or create pull request
- ❌ Changes stay only on their computer


## 3. Add as Collaborator

- ✅ Clone your repo
- ✅ Push changes directly OR
- ✅ Pull request required if **branch is protected**

## Git Feature Branch Workflow

This guide walks through creating a feature branch, making changes, pushing to GitHub, opening a pull request, and pulling merged code.
---
## 📌 Git Script  
``` bash
# Step 1: Create and switch to a new feature branch
git checkout -b feature/my-feature

# Step 2: Stage all changes
git add .

# Step 3: Commit the changes
git commit -m "Add: My feature implementation"

# Step 4: Push the feature branch to GitHub
git push origin feature/my-feature

# 👉 Go to GitHub and open a Pull Request:
#    https://github.com/your-username/your-repo/branches
#    Click “Compare & pull request” next to your branch

# Step 5: (Optional) Pull the latest changes from main after merge
git checkout main
git pull origin main
```

# General Git functions
### ✅ Create a new branch and switch to it
git checkout -b feature/my-feature

### 🔄 Switch to an existing branch
git checkout main

### ✏️ Rename current branch
git branch -m new-branch-name

### ✏️ Rename a specific branch (not checked out)
git branch -m old-branch-name new-branch-name

### 🗑️ Delete a local branch
git branch -d feature/old-feature   # Use -D to force delete locally
git push origin --delete feature1   # delete from github


### 🗑️ Delete a remote branch
git push origin --delete feature/old-feature

```