status:  shows status of the working tree. Indicates 'unsaved changes' that need to be committed and untracked files.

	git status

clone:  clones an existing repository into a new directory. Also creates a branch from the original repo.

	git clone 'link'

add:  adds file to the index. Must be done before changes can be committed  

	git add 'filename' 

rm:  removes files from the index and the working tree. Must be at the end of the branch.

	git rm 'filename'

commit:  'save' changes in the index to the repository

	git commit

push:  used to upload content to a remote repository

	git push origin

fetch:  used to check a remote repository for changes made to it.

	git fetch origin

merge:  used to merge branches together
	
	git merge 'branchname'

pull:  copies changes from a remote repository to the local repository

	git pull origin	

branch:  used to manage branches. Can delete, add, list, etc.

	git branch -d 'branchname'
	git branch 'branchname'
	git branch -a 

checkout:  switches branches 
	
	git checkout 'branchname'

.git folder:  contains information important to the project and a log of commit history

.gitignore file:  a text file that tells git which files or folders to ignore.

Pull requests:  a method of uploading your code to an external repository. Creates a request to be included in the main project that the owner can view and choose to include or deny

SSH authentication to repositories:  ssh provides a secure connection to remote repositories so information can be shared safely.


