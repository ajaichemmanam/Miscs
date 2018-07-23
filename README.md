--TUTORIAL LINK--
Tutorial Link:- https://www.youtube.com/watch?v=xuB1Id2Wxak

--GIT BASICS--
git init //initialise the github repository

git remote add origin ".git link in repository" //link to connect local repo to central repo

git pull origin master // pull repository files

git status // to check status of index of files

git add file.extension // add newly created file to index
git add -A	// to add multiple files to index

git commit -m "any commit message"	//commit message for single file
git commit -a -m "any commit message"	//commit message for all files
// m flag can be avoided, but a popup will ask for adding message.
git log 		//to see the git log file

ssh-keygen		
//used to generate a public ssh key. Used for pushing changes back to repository
// cat the .pub file including path, so you can see the key
// add the generated keys to github account. account-> settings--> SSHandGPG keys --> New SSH KEy (copy paste key) --> Add ssh key
ssh -T git@github.com		// To authenticate the ssh key

git push origin branchname		// used to push the new branch to the remote repository

git checkout hexadecimal filename.fileextension			//hexadecimal: 8 hexadecimal number of commit got from git log
--PARALLEL DEVELOPMENT--
-- BRANCHING--
git branch branchname	//create a branch named branchname

git checkout branchname 	//switch to branch named branchname		//git checkout master to switch back to master branch again

//then add files to that branch using the basic git commands

--MERGING--
git merge branchname 	//merges the branch with branch name as branchname back to master branch

--REBASING--
rebase is used to attach a branch to the master head
git rebase branchname // adds branch to master
git rebase master // adds master to branch

--NOTE--
1. Every branch originates from master and ends in master. 
git stash is used to remove a branch from master temporarily. 
git stash apply is used to reattach the branch back to the master.

2. cat filename	//to see the contents of a file

3.git pull gets all the changed data and merges to master branch of local repository
git fetch gets all the changed data and creates another branch in local repository. and later needs to be applied manually 
