# How to use git

![Logic](#LogifOfGit.png)

1. create Repository online and clone into a folder where you want it

	git clone https://reponame.git

per default the repositroy is created in a directory with the repository name. This can be modified by adding a name after the link, e.g. oldstate

	git clone https://reponame.git oldstate

2. check the status of the Staging Area:

	git status

3. to add a file

	git add file1 file2

if the file is changed it needs to be added again

4. commit file = add it to LOCAL Repository

	git commit -m "Describe the changes"

5. look at all the changes that have happened in the LOCAL repository

	git log

leave `git log` by pressing q

6. push file = add it to the REMOTE Repository

	push file

username is my username
password is my token that I generated for this repository

I only have to put in the password 1x per session
