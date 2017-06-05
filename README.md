# HOW TO USE GITHUB ON UBUNTU

1. Install github
	```Shell
	sudo apt-get install git
	```
2. Cofig github
	```Shell
	git config --global user.name "user_name"
	git config --global user.email "email_id"
	```
3. Create local repository
	```Shell
	git init "repo_name"
	cd "repo_name"
	```
4. Create README file
	```Shell
	gedit README, write something
	```
5. Index file/add file to the staging area 
	```Shell
	git add README
	```
6. Remove files
	```Shell
	git rm file_name  # remove file_name from local and repo
	git rm --cached file_name  # remove file_name from repo ONLY
	```
7. Check repo status
	```Shell
	git status
	```
8. Commit changes
	```Shell
	git commit -m "note"
	```
9. Create a repo at github.com
10. Connect to the created repo
	```Shell
	git remote add origin https://github.com/user_name/repo_name.git
	```
11. Upload/push local files to the github repo
	```Shell
	git push -u origin master
	```
12. Pull down changes
	```Shell
	git pull origin master
	```
13. Check differeces
	```Shell
	git diff
	```
14. Create a new branch
	```Shell
	git branch branch_name
	```
15. Delete branch
	```Shell
	git branch -d branch_name
	```
16. Switch branch
	```Shell
	git checkout branch_name
	```
17. Merge branch
	```Shell
	git branch des_branch # switch to destination branch (the branch to be merged)
	git merge src_branch # merge (des_branch will be a copy of src_branch)
	```
18. Skip enter user and pw every pushing
	```Shell
	$ git config credential.helper store
	$ git push http://example.com/repo.git
	Username: <type your username>
	Password: <type your password>
	```
