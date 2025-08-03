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
 
</ol>