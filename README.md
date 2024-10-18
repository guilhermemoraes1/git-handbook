### git-handbook

Pdf Resource: [git-cheat-sheet](https://education.github.com/git-cheat-sheet-education.pdf)

List of steops

- git --version
	- download git
- git init
- git add
- git commit
	- git config --global user.email "you@example.com"
- create repo on github
	- create a token
- push an existing repository from the command line, copy the commands below
- git remote add origin https://github.com/guilhermemoraes1/git-handbook.git
- gitt branch -M main
- git push -u origin main


git init
turn a directory into a Git project

git status
Check the status of the changes

git add filename
Adds files from the working directory to the staging area

git diff filename
Check the differences between the working directory and the staging area

git commit
commit is the last step, A commit permanently stores changes from the staging area in the repo

git log
shows a list of all previous commits to refer back to an earlier version of a project, Commits are stored chronologically

	git log --oneline shows the list of commits in one line format.

	git log -S "keyword" displays a list of commits 
	where the number of occurrences of the keyword changes within at least one file

	git log --oneline --graph - --graph Displays a visual representation 
	of how the branches and commits were created

git show HEAD
output the most recently made commit (HEAD commit)

git checkout HEAD filename
(be careful)
It'll restore the file in your working directory to look exactly as it did when you last made a commit.

git reset HEAD filename
Unstage that file from the staging area

git reset commit_SHA
works by using the first 7 characters of the SHA of a previous commit.
HEAD is now set to that previous commit.

git reflog
revisit the commits after the git reset
https://discuss.codecademy.com/t/once-we-reset-a-project-to-an-earlier-point-do-the-commits-after-that-point-get-deleted/405699

git stash
when there are 2 branches, use to not lose the changes in this branch, when you go to another branch

git stash pop
when back to the working branch, use this to retrieve the changes you made 

git commit --amend
is useful when updating a commit, it allows to correct mistakes and edit commits easily instead of creating a new one

	git commit --amend --no-edit
	if you want to keep the same commit message, you can simply add the flag --no-edit

ADVANCED
https://www.codecademy.com/courses/learn-git-introduction/articles/handy-git-operations

create alias
git config --global alias.co "checkout"

git co example_branch


https://discuss.codecademy.com/t/what-is-the-difference-between-checkout-and-reset/405720


O que acontece se usar git commit sem a opção -m?
por que usar head em maiusculo?
e o que é head?
por que quando usa o git checkout e git reset tem que usar depois HEAD?
