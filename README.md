**Github CheatSheet**
----------------------------------

Github is a distributed version control system which helps to manage the repositories.

These are a list of few commands that you can use frequently on github(git bash)

```
1.git help
* Take help from github help section for different commands and other errors

```

```
2.git config
* To set the basic configurations on github like your name and email.
```
```
3.git config –global user.name “Pallav chanana”
* Sets configuration values for your user name on git.
```
```

4.git config –global user.email xxxxxx@gmail.com
* Sets configuration values for your user email on git.
```
```

5.git config –global color.ui true
* To see different colours on command line for different outputs.
```
```

6.mkdir folder
* Create a directory if not created initially.

7.cd folder
* To go inside the directory and work upon its contents.

8.git init
* To create a local git repository for us in our folder folder.This will help to manage the git commands for that particular repository.
```
```

9.git status
* To see whats changed since last commit.It shows all the files that have been added and modified and ready to be commmitted and files which are untracked
```
```

10.git add Readme.txt
* To add a file Readme.txt to the staging area to track its changes.
```
```

11.git commit -m “Created a Readme.txt”
* To commit our changes(taking a snapshot) and providing a message to remember for future reference.
```
```
12.git log
To check the history of commits for our reference.
```
```

Here are Different ways to use add command to move files to staging area:

13.git add
T* o add a specific list of files to staging area.

14. git add *.txt
To add all text files of the current directory to staging area.

15. git add --all
To add all files of current directory to staging area.
Note-
i)Do not use this command directly ensure every file if right.
ii) Sometimes gitignore file is not modified to ignore unrequired files like eg: logs etc 


16.git add docs/*.txt
* To add all text files of a particular directory(docs) to staging area.

17.git add docs/
* To add all files in a particular directory(docs) to staging area.

18.git add “*.txt”
* To add text files of entire project to staging area.
```
```

More Commands:

19.git diff
* To figure out what changes you made since last commit.
```
```

20.git reset head new-branch
* To undo staging of the file that was added in the staging area.
```


```

21.git checkout –new-branch
* To Blow away all changes since the last commit of the file.
```
```

22.git commit -a -m “Readme.md”
* To add any of our tracked files to staging area and commit them by providing a message to remember.
```
```

23.git reset –soft HEAD^
* To undo last commit and bring file to staging area.
```
```

24.git reset –hard HEAD^
* To undo last commit and remove file from the staging area as well(In case we went horribly wrong).
```
```

25.git reset –hard HEAD^^
* To undo last 2 commits and all changes.
```
```

26.git remote add origin https://github.com/pallavchanana/git-cheatsheet.git
* This commands make a bookmark which signifies that this particular remote refers to this URL.
This remote will be used to pull any content from the directory and push our local content to the global server.
```
```

27.git remote add <address> 
To add new remotes to our local repository for a particular git address.
```
```

28.git remove rm
* To remove a remote from our local repository.
```
```

29.git push -u origin master
* To push all the contents of our local repository that belong to master branch to the server(Global repository).
```
```

30.git clone <https://github.com/pallavchanana/git-cheatsheet.git>
* To clone or make a local copy of the global repository in your system
(git clone command downloads the repository and creates a remote named as origin which can be checked by command – git remote -v).
```


```

31.
i. git branch new-branch
* To create a new branch named as new-branch.
OR 
ii. git checkout -b new-branch
* To create a new branch named as new-branch.

```
```

32.git branch
* To see all the branches present and current branch that we are working on.
```
```

33.git checkout new-branch
* T* o switch to branch new-branch from master branch.
```
```

34.ls
To see directories and files in the current directory.
```
```

35.git merge new-branch
* To merge new-branch branch with master branch.
```
```

36.git branch -d new-branch
T* o delete new-branch branch.
```
```
37.git checkout -b admin
* To create a new branch admin and set it as current branch.
```
```
38.git branch -r
To look at all the remote branches.
```
```
39.git branch -D new-branch
* To forcefully delete a branch without making commmits.
```
```
40.git tag
* To see the list of available tags.
```
```
41.git checkout v1.0.0
* To set the current tag to v1.0.0.
```
```
42.git tag -a new-branch -m “new-branch 1.0”
* To create a new tag.
```
```
43.git push –tags
* To push the tags to remote repository.
```
```
44.git fetch
* To fetch down any changes from global repository to current repository
```
```
45.git rebase
* Move all changes to master which are not in origin/master to a temporary area.
* Run all origin master commits.
* Run all commits in the temporary area on top of our master
```
```
46. git commit —amend -m "fixing a typo" 

* git commit -m "fixing a typeo" and hit "Enter". Quickly we realize that not only were we trying to fix a typo in the application, but now we need to fix the "typeo" in the commit message.

* Running the command git commit —amend -m "fixing a typo" does the trick. Now when our push our commit, our co-workers won’t see that our "typo" was original spelled "typeo".

```
```
47. git cherry-pick
* we can pick a particular branch that has a commit and pull it into another. Let’s walk through this.

*Let’s say we have a branch branch-test and we have committed all of our changes. There’s another branch, we’ll just use master but this can be any branch, and we want to pull in branch-test’s commit. By using the command, git cherry-pick branch-test we can get that entire commit into another branch.