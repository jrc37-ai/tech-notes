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

### Conecting to a specific repository in github
```
git remote add origin <Github repository URL>
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

### Stage all the changes 
```
git add .
```

### Commit all the changes
```
git commit -m "COMMENTARY"
```

### Upload the changes to the GitHub repository
```
git push origin main
```
