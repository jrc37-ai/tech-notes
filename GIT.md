# GIT

### Install git from https://git-scm.com/

### Verify git is correctly installed by checking version.
```
git --version
```

### Initialize the repository
```
git init
```

### Configure the user data as global features
```
git config --global user.email <email>
git config --global user.name <name>
```

### Check if local folder is empty about remote tracking
#### Inf nothing appears, we can add the remote repository
```
git remote -v
```

### Conecting to a specific repository in github
```
git remote add origin <Github repository URL>
```

### In case that the Github repository has already a `.gitignore` file
```
git pull origin main
```

### Stage all the changes 
```
git add .
```

### Commit all changes
```
git commit -m "COMMENTARY"
```

### Commit with automatic staging of the files
```
git commit -a -m "COMMENTARY"
```

### Stop tracking a file
#### First of all, it's neccesary to stop tracking a file, in order for it to disappear from the repository, even when that file is already included in the .gitignore file.
```
git rm --cached FILENAME
```

### Stop tracking a folder
```
git rm --cached -r FOLDERNAME
```

### Add changes to the last commit 
**Not recommendable when syncing with a remote repository like GitHub.
```
git commit --amend
```
### Modify comment of the last commit 
```
git commit --amend -m "Updated commit message"
```

### Upload the changes to the GitHub repository
```
git push origin main
```

### Create a new branch and switch to it
```
git checkout -b BRANCH_NAME
```
Unfolded way to do this:
```
git branch BRANCH_NAME
git checkout BRANCH_NAME
```

### Merge a branch into master branch
```
git checkout master
git merge BRANCH_NAME
```

### Delete a branch
```
git branch -d BRANCH_NAME
```

### See all local and remote branches
```
git branch -a
```
