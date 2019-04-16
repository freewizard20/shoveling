# Git essentials

1. git reset HEAD ~ file : unstage file
2. git rm -r {{directory}} : stage deleted files
3. git rev-parse HEAD : check current HEAD

## git set new url

1. git remote -v : check current remote origin
2. git remote set-url origin https://github.com/.... : change git url

## git compare commits with local/remote

1. git diff master origin/master

## git check branch status

1. git checkout --track origin/master

## git merge



## git config

1. git config --global user.name "jinhyuk.jeon"
2. git config --global user.email "freewizard@freewizard.net"


## using git

* basic configs(required on first use)

`git config --global user.name "{{username}}"`
    
 `git config --global user.email "{{email}}"`

* stage changes

`git add *`

* stage deletes also

`git add -u`

* commit changes

`git commit -m "{{message with commit}}"`

* undo commits

`git commit -m "{{reverting message}}`

* make new branch

`git branch {{newbranch}}`

* check all branch lists

`git branch -r`

* move to new branch

`git checkout {{branch-to-go}}`

* merge branches ( first be at branch to receive merge )

`git merge {{branchname}}`

* receive updates from remote

`git pull`

* update changes to remote

`git push origin master`

* update changes to local

`git fetch -p`



