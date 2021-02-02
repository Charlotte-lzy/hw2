List all the git commands (only the commands that start with `git` and nothing else), in order that you needed to execute them, to carry out the scenario in Task-4, below.\
**add two different course number to Github and local repository**\
`git init`\
`git status`\
`git add .`\
`git commit -m "Creat README.md write name"`\
`git remote add origin https://github.com/Charlotte-lzy/task4.git` \
`git branch -M main`\
`git push -u origin main`\
`git add .`\
`git commit -m "add course name 621"`\
**solve conflict**\
`git pull origin main`\
`git add .`\
`git commit -m "change course name 421/621"`\
`git push origin main`\
**merge two branches**\
`git branch new-feature`\
`git checkout new-feature`\
`git push --set-upstream origin new-feature`\
`git pull origin main`\
**fix bugs**\
`git branch bug-1`\
`git branch bug-2`
`git checkout bug-1`\
`git add .`\
`git commit -m “Working on bug-1”`\
`git stash`\
`git checkout bug-2`\
`git add .`\
`git commit -m "Fixed bug-2"`\
`git stash pop`\
`git add .`\
`git commit -m "Fixed bug-1"`\
`git checkout main`\
`git branch -a`\
`git push --all origin`\