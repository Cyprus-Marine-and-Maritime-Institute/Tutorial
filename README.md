
# Git Github Tutorial

## Initialize the git repository
```bash
git init
```
## Create the gitignore file
The .gitignore file is a file that is used to determine which files and directories to ignore in a project. It helps you keep your repository clean by excluding files that you don't want to track or share, such as build outputs, temporary files, or files containing sensitive information.

```bash
touch .gitignore
```
Alternatively create the .gitignore file within you file explorer of choice or through Visual Studio Code

## Initialize the github repository

1. Navigate to [github.com](https://github.com/Cyprus-Marine-and-Maritime-Institute)
2. Go to Repositories
3. Click on New repository (Upper right corner)
4. Name the repository and choose if the repository will be public or private (Always choose private except if instructed otherwise)
5. Make sure the Owner is Cyprus-Marine-and-Maritime-Institute
6. Create the repository (Scroll down and click (Create repository) )

## Back in your codebase

```bash
git add ./ #if you decide to run this make sure your .gitignore is setup correctly
```

```bash 
git add <your_files.py> # add one by one files or folders
git commit -m "<your commit message>"
git branch -M main # switch to the main branch
git remote add origin https://github.com/Cyprus-Marine-and-Maritime-Institute/test2.git # add the local branch to the remote branch
git push -u origin main #sync the local branch to the remote branch
```

## Branches
### List available branches
```bash
git branch
```
### Create a new branch
This will be created only as a local branch
```bash
git branch <new branch name>
```
### Switch to Local branch
```bash
git checkout <new branch name>
```
### Create the branch to the remote repository
```bash
git push --set-upstream origin <new branch name>
```

## Merging

After making changes to the new branch if would like to merge them with the main branch these are the following steps

1. **Make sure you are in your project directory.**
2. **Switch to branch you would like to merge into**
 ```bash 
git merge <branch name the changes are coming from>
```
3. Resolve any Conflicts through the visual studio code visual editor
4. Commit the changes
```bash
git commit -m <Message to commit>
```
5. Push the local change to the repository
```bash
git push
```
