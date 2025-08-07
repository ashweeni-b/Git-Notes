## Command Used for the Project

The Git commands used to complete the tasks are as follows:

<ol>

<li> <code> git --version </code> </li>
Tells the version of Git installed in the system. <br> <br>

<li> <code> git init </code> </li>
- Used to initialize the current repository as git repository. <br>
- Creates an empty repository in the current directory. <br>
- The current directory becomes the default master branch. <br>
- <i> .git </i> file is created in the directory after initialization of the repository as the Git repository. <br>
- <i> .git </i> file is the hidden file in the directory. <br> <br>

<li> <code> git status </code> </li>
Used to get the current status of the repository. <br> <br>

<li> <code> git add [file_name] </code> </li>
Used to add the modified <i> file_name </i> to the staging area. <br> <br>

<li> <code> git add . </code> </li> 
Used to add all the modified files in the staging area. <br> <br>

<li> <code> git rm --cached [file_name] </code> </li>
Used to unstage the <i> file_name </i> from the staging area. <br> <br>

<li> <code> git commit -m "message" </code> </li>
Used to commit the staged files with a message. <br> <br>

<li> <code> git commit </code> </li>
Used to commit the staged files using the set/default code editor. The commit message is written with the help of the default code editor. <br> <br>

<li> <code> git commit -am "message" </code> </li>
Used to stage and commit the file simultaneously with a message. <br> <br>

<li> <code> git config --global user.email [email_id] </code> </li>
Used to set the <i> email-id </i> of the user. <br> <br>

<li> <code> git config --global user.name [user_name] </code> </li>
Used to set the <i> user-name </i> of the user. <br> <br>

<li> <code> git config --global user.email </code> </li>
Used to check the <i> email-id </i> of the user. <br> <br>

<li> <code> git config --global user.name </code> </li>
Used to check the <i> user-name </i> of the user. <br> <br>

<li> <code> git log </code> </li>
Used to get commit history. <br> <br>

<blockquote> 
Every commit is assigned with a SHA-1 (40 character) key, a hexadecimal key. <br>
Commit key is generated depending on the contents of the file. </li>
</blockquote> <br>

<li> <code> git log --oneline </code> </li>
Used to get commit history in short form - 7 character SHA-1 key and a one line commit message. <br> <br>

<li> <code> git show HEAD </code> </li>
Used to get detailed commit history about the HEAD branch. <br> <br>

<li> <code> git show [commit-id] </code> </li>
Used to get the detailed commit history for the provided commit-id. <br> <br>

<li> <code> git show HEAD~n </code> </li>
Used to get the detailed commit history for the nth commit-id. <br> 
E.g. <code> git show HEAD~3 </code> - Shows commit history of the 3rd commit.<br> <br>

<li> <code> code . </code> </li>
Used to run the current directory in the default code editor. <br> <br>

<li> <code> code [repository_name]/ </code> </li>
Used to run the repository <i> repository_name </i> in the default code editor. <br> <br>

<li> <code> code [file_name] </code> </li>
Used to run the file <i> file_name </i> in the default code editor. <br> <br>

<li> <code> code ~/.git config </code> </li>
Used to check the configuration set for the Git. Gives information about the username, email and editor. <br> <br>

<li> <code> git [topic] --help </code> </li>
Used to get information regarding the <i> topic </i> in the new tab. <br> <br>

<li> <code> git checkout [file_name] </code> </li>
Used to unmodify/revert the changes in the <i> file_name </i>. <br>
Used after the files are modified but before the staging area. <br> <br>

<li> <code> git checkout . </code> </li>
Used to unmodify/revert the changes in all the files present in the directory. <br> <br>

<li> <code> git checkout [commit_id] </code> </li>
Opens the <i> commit_id </i> as the HEAD. <br>
The HEAD is detached head i.e. it is detatched from the master branch and it is attached to the <i> commit_id </i>. <br>
The <i> commit_id </i> and the <i> commit_message </i> is seen once the HEAD is attached to the <i> commit_id </i>. <br>
Status of the project during that <i> commit_id </i> is retrieved back. <br>
To go back to the master branch, use <code> git checkout master </code>. <br> <br>
Any modifications made in the detatched HEAD does not get saved, which means it does not exists once moved to the master branch. <br> <br>
 
<li> <code> git revert [commit_id] </code> </li>
Undo the specific commit with the given <i> commit_id </i>. <br>
No other commits are disturbed, while reverting the specific commit. <br> 
A new commit with the revert changes appears in the log history. <br> <br>

<li> <code> git reset --mixed [commit_id] </code> </li>
Remove the commits and files are in the unstaged area. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset --soft [commit_id] </code> </li>
Remove the commits and files are in the staging area. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset --hard [commit_id] </code> </li>
Remove the commits and files directly. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset . </code> </li>
Remove the commits and follows the <code> git reset --mixed </code> command. <br> <br>

<blockquote>
<b> How to ignore files in Git? </b> <br>
1. Create a <i> .gitignore </i> file in the project folder. <br> <br>
2. Add the file names to be ignored in the format as follows : <br>
(a) [folder_name]/[file_name] - If files are present in different folders <br>
(b) /[file_name] - If files are present in the same folder <br>
(c) /*.[extension] - If more files with same extension is present and we have to ignore them at once 
</blockquote> <br>

<li> <code> git remote add origin [https-link-of-repository] </code> </li> 
Used to connect local repo to the remote repo. <br>
The https-link of the remote repo is used. <br> <br>

<li> <code> git remote remove origin </code> </li> 
Removes the connection of local repo and remote repo. <br> <br>

<li> <code> git remote -v </code> </li> 
Used to check the connected remote repos. <br> <br>

<li> <code> git branch --set-upstream-to=origin/[branch] main </code> </li> <br>
Links local branch to the remote branch so that Git knows which branch to pull from and push to by default. <br>
In Git, the upstream branch is the default remote branch that your current local branch is tracking. <br>
origin/[branch] is the remote branch and main is the local branch. <br>
Set the local branch main to track the remote branch origin/[branch]. <br>
After setting this branch, we can directly use <code> git pull </code> and <code> git push </code> <br> <br>

<li> <code> git push origin main </code> </li> 
Used to push the content from local repo to the remote repo. <br>
Push the content to the origin main branch of the remote repo. <br> <br>

<blockquote>
Instead of setting the upstream branch, alternatively we can use <code> git push -u origin main </code> at the first time while pushing the content into the remote repo. <br>
This not only pushes the content, but also sets the upstream branch as the origin main branch. </br> 
So, after that we can directly use <code> git push </code> and <code> git pull </code> for pushing and pulling of content to and from remote repo.
</blockquote> <br>

<li> <code> git push </code> </li> 
Used to push the content from local repo to the set branch of the remote repo. <br> <br>

<li> <code> git pull origin main </code> </li> 
Used to pull the content from renote repo to the local repo. <br>
Pull the content from the origin main branch of the local repo. <br> <br>

<li> <code> git pull </code> </li> 
Used to pull the content from the set branch of remote repo to the local repo. <br> 

</ol>