# Git Important Commands

#### How to get current user
``` git config user.name ```

#### How to get remote url for a repo
``` 
go to repository and hit below command
git config --get remote.origin.url 

```

#### How to take checkout in git
``` git clone REPO_URL ```

#### List out all branches 
```  git branch -l ```

#### Start new repo locally
``` 
go to folder

git init
git add .   (here . dot means all files in directory you can specify special files)
git commit -m "initial commit"   (This command will commit code locally)
git remote add origin remote_repo_url (connect local repo to remote repo)
git push   (Push commited changes to remote repo)
```

#### Show current branch Git
``` git branch ```

#### Create git branch 
``` git branch BRANCH_NAME```

#### Switch to another branch
``` git checkout BRANCH_NAME```

#### Show current changes in files
``` git status```

#### Add new file in repo
``` git add FILE_NAME or  . (dot will all new file in current dir) ```

#### Add changes in current repo
``` git stageg . (dot will added all changed file,specific file name can be used ) ```


#### Git clone specific branch only 
```  git cline CLONE_URL BRANCH_NAME  ```

#### Checkout master branch
``` git checkout master ```





