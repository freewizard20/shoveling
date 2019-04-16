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

## git config

1. git config --global user.name "jinhyuk.jeon"
2. git config --global user.email "freewizard@freewizard.net"

## stage changes

1. git add *
2. git add -u

## commit changes

1. git commit -m "{{message with commit}}
2. git commit -m "{{reverting message}}

## branch management
1. git branch {{newbranch}}
2. git checkout {{branch-to-go}}
3. git checkout -b newbranch // make new branch and checkout at once

## merge
1. git merge {{branchname}}
2. git fetch -p // update branches (?)



