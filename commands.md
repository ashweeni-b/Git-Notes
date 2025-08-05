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
To back to the master branch, use <code> git checkout master </code>. <br> <br>
Any modifications made in the detatched HEAD does not get saved, which means it does not exists once moved to the master branch. <br> <br>
 
<li> <code> git revert [commit_id] </code> </li>
Undo the specific commit with the given <i> commit_id </i>. <br>
No other commits are disturbed, while reverting the specific commit. <br>

<li> <code> git reset --mixed [commi_id] </code> </li>
Remove the commits and files are in the unstaged area. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br>

<li> <code> git reset --soft [commi_id] </code> </li>
Remove the commits and files are in the staging area. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br>

<li> <code> git reset --hard [commi_id] </code> </li>
Remove the commits and files directly. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br>

</ol>