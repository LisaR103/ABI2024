# How to use git

![Logic](https://github.com/LisaR103/ABI2024/blob/main/LogicOfGit.png)

1. create Repository online and clone into a folder where you want it

	`git clone https://reponame.git`

per default the repositroy is created in a directory with the repository name. This can be modified by adding a name after the link, e.g. oldstate

	`git clone https://reponame.git oldstate`

2. check the status of the Staging Area:

	`git status`

3. to add a file

	`git add file1 file2`

wildcards apply, e.g. *.txt etc to add several files at once
if the file is changed it needs to be added again

4. commit file = add it to LOCAL Repository

	`git commit -m "Describe the changes"`

5. look at all the changes that have happened in the LOCAL repository

	`git log`

leave `git log` by pressing q
the commit showing origin/main Head/main is where the remote repository is

6. push file = add it to the REMOTE Repository

	`push file`

username is my username
password is my token that I generated for this repository

I only have to put in the password 1x per session

7. getting back an old version after a mistake = going back to that commit

	`git checkout [commitnumber]`

everything I do now happens with the state of the files at this snapshot, but I can't commit these files
what I can do is copy it into the parent directory and later back in
to go back to the most current:

	`git checkout main`

8. gitignore

files that I don't want versions because it is a waste of space and clusters the repositroy
e.g. pdf files/result files

I can add all of those file to a file called `.gitignore`

This is a text file without a file extension

contant e.g.:
.*
!.gitignore

= ignore everything that starts with a `.` except `.gitignore` itself

9. turning a markdown file into a pdf file

	`pandoc -o file.pdf file.md`

## Branching

This is to have a "work in progress" save so you don't change the main

Create branch: `git checkout -b branchname` (if it doesn't exist)
Commit the branch: `git commit -m "message"`
Push the branch: `git push -u origin branchname`

Merge two branches (here branchname with master ):
`git checkout master`
`git merge branchname (In case of conflict: Edit, commit

## Tags
Adding a license in important!!! Even if it's just to have a liability statement
