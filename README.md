# learn_git

## git commands

### Create A git Repo

```bash
# create brand new repositories (repos) on your computer
git init

# clone or copy existing repos from somewhere else to your local computer
git clone
# $ git clone <path-to-repository-to-clone>
#cloning the repo with default name (Example), It creates directory with name course-git-blog-project in current directory
git clone https://github.com/udacity/course-git-blog-project

#cloning the repo using new name instead of default one (Example), It creates directory with name blog-project in current directory
git clone https://github.com/udacity/course-git-blog-project blog-project

# check the status of a repo
git status
```

### Review a Repo's History

```bash
#Display information about the given commit (we have to provide sha i.e. commit ID with it)
git show

#displays information about the existing Commits
git log

###flags with git log command
#displays information int one line, shows the first 7 characters of the commit's SHA,shows the commit's message
git log --oneline

#displays the file(s) that have been modified, displays the number of lines that have been added/removed, displays a summary line with the total number of modified files and lines that have been added/removed
git log --stat


#displays the files that have been modified, displays the location of the lines that have been added/removed, displays the actual changes that have been made
git log -p


#display the patch information, but will not highlight lines where only whitespace changes have occurred.
git log -p -w
```

# Add Commits To A Repo

```bash
#Add files from the working directory to the staging index
git add . or <filename>   #Filename in case of specific file and . in case of all files and directories in current directory

#Remove files from staging index
git restore --staged <filename>

#take files from the staging index and save them in the repository
git commit

#flage with git commit -m (for adding commit message or discription to it)
git commit -m 'commit message'

#displays the difference between two version of file
#displays the files that have been modified, the location of the lines that have been added/removed, the actual changes that have been made
git diff

#Untracked files -- make .gitignore file (enter name of all files you want to ignore by git)
```
