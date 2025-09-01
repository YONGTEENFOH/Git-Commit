How to initialize a local repo, remote add repo, commit with specific date and push the changes.

#Create a local folder in desktop

#open the the folder in vscode

#login to github from vscode

git init

git add .

git commit --date='2025-11-01' -m 'editing readme file'

#make sure winget is installed in win11, if not, run CMD in admin, winget install --id GitHub.cli

gh auth login

gh repo create [name-of-your-repo] --public --source=. --push

#If you omit the [name-of-your-repo], it defaults to the current directory name.

#Use --private or --internal instead of --public for different visibility settings.

#The --source=. flag specifies the local directory to use as the source, and --push automatically pushes your local commits to the new remote. 

git remote add origin https://github.com/YONGTEENFOH/Git-Commit

git push --set-upstream origin1 master

#after upstream is set, you can use git push only to push any changes