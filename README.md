# Git Important Commands

#### How to take checkout in git
``` 
git clone REPO_URL 
```

#### List out all branches 
```  
git branch -l 
```

#### Start new repo locally
go to repo folder
``` 
git init
git add .   (here . dot means all files in directory you can specify special files)
git commit -m "initial commit"   (This command will commit code locally)
git remote add origin remote_repo_url (connect local repo to remote repo)
git push origin master  (Push commited changes to remote repo)
git push origin feature_branch
```

#### How to get current user
``` 
git config user.name 
```

#### How to get remote url for a repo
Go to repository and hit below command
``` 
git config --get remote.origin.url 
```

#### Show current branch
``` 
git branch 
```

#### Create git branch 
```
git branch -b BRANCH_NAME
```

#### Switch to another branch
```
git checkout BRANCH_NAME
```

#### Show current changes in files
```
git status
```

#### Add new file in repo
dot will add new file in current dir
```
git add FILE_NAME or  . 
```

#### Add changes in current repo
dot will add all changed file,specific file name can be used 
```
git stage . 
```

#### Git clone specific branch only 
```
git clone CLONE_URL BRANCH_NAME  
```

#### Checkout master branch
```
git checkout master 
```

#### Git remove remote origin 
```
git remote rm origin 
```
 
#### Git remove fie
``` 
git rm -r --cached FILE_NAME (It will remove file from git repo )
git commit 
git push  (After psuh file will be deleted from remote branch)  
```
Note: file is delted from local git and remote git repo but file exist in your local directory but it is 
no longer of your git repo you can delete it from you file system


#### Discard all local changes which are not staged yet
It will discard all local changes but it stores changes to temrory file which can later be restored
```
git stash 
```


### Permanently discard local changes
```
git checkout -- <file>  (It will permanently remove local changes)
```

#### Show stashed changes list
Lists all previously stashed commits (yes, there can be more) that were not poped
```
git stash list 
``` 


#### Redoes previously stashed changes and removes them from stashed list
```
git stash pop 
``` 

#### Redoes previously stashed changes, but keeps them on stashed
```
git stash apply 
```
  
#### How to unstage everything but keep changes (Not commited yet)
 ```
 git reset (This will remove changes from staging)
 ```

#### How to unstage everything dont keep changes (Not commited yet)
 ```
 git reset --hard FILE_NAME (This will remove changes from staging)
 ```

#### Unstage the file to current commit (HEAD)
 This will remove changes from staging also we can say it will bring file to current commit condition
 ```
 git reset HEAD FILE_NAME 
 ```

#### How to discard all local changes, but save them for later (Not staged yet)
```
git stash 
```

#### How to revert recently commit changes
```
git reset --hard HEAD~1 (It will set your file to previous commit) 
>alternativly
git reset --hard COMMIT_ID 
```    
#### View all commit history
```
git log
```

#### How to delete branch at localy and remotely
```
git branch -d BRANCH_NAME

git push <remote_name> --delete <branch_name>
```

#### Create branch and take checkout from feature branch
```
git checkout -b FEATURE_BRANCH_1 FEATURE_BRANCH_2
```

#### How to create tag in Git
```
git tag -a v1.4 -m "my version 1.4"
git push origin v1.4
```
#### Git refusing to merge unrelated histories on rebase
```
git pull origin master --allow-unrelated-histories

```

### Difference between git pull and fetch

```
git fetch will bring metadata from remote branch it will not transfer any file it just update if there is any commit on remote branch

git pull will actually pull data and merge them with local branch
```
