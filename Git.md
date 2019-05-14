# Git

## git useful links
1. [git documentation](https://git-scm.com/about)
2. [git tutorial](https://backlog.com/git-tutorial/kr/)

## commands
1. git reset HEAD ~ file : unstage file
2. git rm -r {{directory}} : stage deleted files
3. git rev-parse HEAD : check current HEAD
4. git log origin/master
5. git log --pretty=format:"%h %s" --graph
6. git remote -v : check current remote origin
7. git remote set-url origin https://github.com/.... : change git url
8. git rm -r --cached .
9. git add .
10. git commit -m ".gitignore fix"
11. git diff master origin/master
12. git checkout --track origin/master
13. git config --global user.name "jinhyuk.jeon"
14. git config --global user.email "freewizard@freewizard.net"
15. git add *
16. git add -u
17. git commit -m "{{message with commit}}
18. git commit -m "{{reverting message}}
19. git branch {{newbranch}}
20. git checkout {{branch-to-go}}
21. git checkout -b newbranch // make new branch and checkout at once
22. git merge {{branchname}}
23. git fetch -p // update branches (?)
