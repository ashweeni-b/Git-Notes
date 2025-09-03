## Commands in Git

The Git commands are as follows:

<ol>
<h3> <i> Help & Info </i> </h3>

<li> <code> git --version </code> </li>
Provides the current version of Git installed in the system. <br> <br>

<li> <code> git help </code> </li>
Provides general help. <br> <br>

<li> <code> git [command] --help </code> OR <code> git help [command] </code> </li>
Provides information about the <i> command </i> in the new tab. <br>

</ol>

____ 

<ol>
<h3> <i> Repository Setup </i> </h3>

<li> <code> git init </code> </li>
- Initializes the current repository as an empty git repository by creating a .git file in the repository. <br>
- The current directory becomes the default master or main branch. <br>
- <i> .git </i> file is the hidden file in the directory. <br> <br>

<li> <code> git config --global user.email [email_id] </code> </li>
Sets the <i> email-id </i> of the user. <br> <br>

<li> <code> git config --global user.name [user_name] </code> </li>
Sets the <i> user-name </i> of the user. <br> <br>

<li> <code> git config --global user.email </code> </li>
Provides the <i> email-id </i> of the user. <br> <br>

<li> <code> git config --global user.name </code> </li>
Provides the <i> user-name </i> of the user. <br> <br>

<li> <code> code ~/.git config </code> </li>
Shows the current configuration set for the Git. Gives information about the username, email and editor. <br> <br>

<li> <code> git clone [url_of_repository] </code> </li>
Clones a remote repository locally. <br> 

</ol>

____

<ol>
<h3> <i> Basic Workflow </i> </h3>

<li> <code> git status </code> </li>
Provides the current status of the repository. <br> <br>

<li> <code> git add -A </code> </li>
Stages all the changes. <br> <br>

<li> <code> git add . </code> </li> 
Stages new and modified files. <br> <br>

<li> <code> git add -u </code> </li>
Stages modified and deleted files only. <br> <br>

<li> <code> git add [file_name] </code> </li> 
Stages a specific file. <br> <br>

<li> <code> git commit -m "message" </code> </li>
Commits the staged files with a message in the command line interface. <br> <br>

<li> <code> git commit </code> </li>
Commits the staged files using the set/default code editor. The commit message is to be written with the help of the default code editor. <br> <br>

<li> <code> git commit -am "message" </code> OR <code> git commit -a -m "message" </code> </li>
Stages and commits the file simultaneously with a message. <br> 
This command works only for modified and updated files and not for newly created files. <br> <br>

<li> <code> git log </code> </li>
Provides the commit history in detailed format. <br> <br>

<blockquote> 
Every commit is assigned with a SHA-1 (40 character) key, a hexadecimal key. <br>
Commit key is generated depending on the contents of the file. <br>
</blockquote> <br> 

<li> <code> git log --oneline </code> </li> 
Provides the commit history in short format - 7 character SHA-1 key and a one line commit message. <br> <br>

<li> <code> git log --oneline --graph </code> </li>
Views concise branch history in the form of graphs. <br> 

</ol>

____

<ol>
<h3> <i> Inspecting Changes </i> </h3>

<li> <code> git diff </code> </li>
Provides the difference between current working directory and the staging area. <br> <br>

<li> <code> git diff --staged </code> OR <code> git diff --cached </code> </li>
Provides the difference between staging area and the last committed version. <br> <br>

<li> <code> git diff [commit_1] [commit_2] </code> </li>
Provides the difference between commits. <br> <br>

<li> <code> git diff [branch_1] [branch_2] </code> </li>
Provides the difference between the tips of two branches. <br> <br>

<li> <code> git diff [commit/branch] </code> </li>
Provides the difference between current working directory and the commit or the branch. <br> <br>

<li> <code> git show [commit_id] </code> </li>
Provides the changes of a specific commit_id. <br> 

</ol>

____

<ol>
<h3> <i> Undoing Changes </i> </h3>

<li> <code> git checkout -- [file_name] </code> </li>
Reverts or unmodifies the changes in working directory. <br>
Used after the files are modified but before the staging area. <br> <br>

<li> <code> git checkout . </code> </li>
Reverts or unmodifies the changes in all the files present in the directory. <br> <br>

<li> <code> git restore [file_name] </code> </li>
Discards the changes in the working directory. <br>
Newer alternative to checkout for files. <br> <br>

<li> <code> git reset --soft [commit_id] </code> </li>
Move HEAD and keep the changes staged. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset --mixed [commit_id] </code> </li>
Move HEAD and keep the changes unstaged. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset --hard [commit_id] </code> </li>
Remove the commits and files directly. <br>
The <i> commit_id </i> is the id upto which we need to remove the commit. <br> <br>

<li> <code> git reset . </code> </li>
Moves HEAD and keep the changes unstaged. <br> 
It is similar to <code> git reset --mixed </code> <br> <br>

<li> <code> git revert [commit_id] </code> </li>
Safely creates a new commit that undoes the previous commit. <br> <br>

<li> <code> git clean -fd </code> </li>
Remove untracked files and folders. <br>

</ol>

____

<ol>
<h3> <i> Branching and Merging </i> </h3>

<li> <code> git branch [branch_name] </code> </li>
Creates a new branch <br> <br>

<li> <code> git branch </code> </li>
Lists the branches in the project. <br>
The current branch is highlighted with a '*' and is in green color. <br> <br>

<li> <code> git branch -D [branch_name] </code> </li>
Deletes the branch locally. <br> <br>

<li> <code> git checkout [branch_name] </code> </li>
Switches between the branches. <br> <br>

<li> <code> git checkout -b [branch_name] </code> </li>
Creates a new branch <i> branch_name </i> and switch to it. <br> <br>

<blockquote>
In Git, the modifications made by specific branches are not seen in other branches until and unless the branches all are merged.
</blockquote> <br> 

<li> <code> git switch <branch> </code> </li>
Newer alternative to checkout for branches. <br> <br>

<li> <code> git merge [branch_name] </code> </li>
Merges the branch with the main branch </i>. <br> 
Used to combine branches by preserving history. <br> <br>

<li> <code> git merge --abort </code> </li>
Aborts the merging of the branch with the main branch. <br> <br>

<li> <code> git rebase [branch_name] </code> </li>
Combines the branch with the main branch. <br>
Used to combine branches by rewriting history. <br> <br>

<blockquote>
<i> main: </i> A -> B <br> <br>
<i> feature1: </i> A -> B -> C -> D <br>
<i> main: </i> A -> B -> E -> F <br> <br>

After rebasing, the feature1 branch becomes, <br>
<i> feature1: </i> A -> B -> E -> F -> C' -> D' <br>
- The <i> main </i> branch was 2 commits ahead of <i> feature1 </i> branch, so rebasing the branch, adds the commits from the main branch into the <i> feature1 </i> branch. <br>
- In log history of <i> feature1 </i> branch, we can see the commits of <i> main </i> branch also. But in the history of <i> main </i> branch we are not able to see the commits from the <i> feature1 </i> branch, so for that we need to merge these two branches.
</blockquote> 

</ol>

____

<ol>
<h3> <i> Remote Repositories </i> </h3>

<li> <code> git remote add origin [url_of_repository] </code> </li> 
Connect local repo to the remote repo. <br>
The https-link of the remote repo is used. <br> <br>

<li> <code> git remote -v </code> </li> 
List the remote repos. <br> <br>

<li> <code> git remote remove origin </code> </li> 
Removes the connection of local repo and remote repo. <br> <br>

<li> <code> git push -u origin [branch_name] </code> </li>
- Pushes the branch to remote repo with the help of upstream. <br>
- Also, sets the upstream branch as the origin main. <br>
- After setting the upstream branch we can directly push or pull to and from the remot repo. <br> <br>

<li> <code> git push origin main </code> </li> 
Pushes the local repo to the remote repo. <br>
The content from the origin main branch is psuhed to the remote repo. <br> <br>

<li> <code> git push </code> </li> 
Push the commits. <br> <br>

<li> <code> git pull origin main </code> </li> 
Fetches or merges from remote repo to the local repo. <br>
The content from the remote repo is fetched or merged into the remote repo. <br> <br>

<li> <code> git pull </code> </li> 
Fetches and merges the commits from the remote repo. <br> <br>

<li> <code> git fetch </code> </li>
Fetch changes from the remote repo, without merging the changes. <br> <br>

<li> <code> git push origin [branch_name] </code> </li>
Pushes the locally created branch to the remote repo. <br> <br>

<li> <code> git pull origin [branch_name] </code> </li>
Pulls the remotely created branch to the local repo. <br> <br>

<blockquote>
In Git, the remotely pulled repo is not seen in the local repo until we track the repos. <br>
</blockquote> <br> 

<li> <code> git push origin --delete [branch_name] </code> </li>
Remotely deletes the branch from the local repo. <br> <br>

<blockquote>
Branch deleted locally, does not delete the branch remotely. And branch deleted remotely, does not delete the branch locally. 
</blockquote> <br> 

<li> <code> git branch --set-upstream-to=origin/[branch] main </code> </li> <br>
- Links local branch to the remote branch so that Git knows which branch to pull from and push to by default. <br>
- In Git, the upstream branch is the default remote branch that your current local branch is tracking. <br>
- origin/[branch] is the remote branch and main is the local branch. <br>
- Set the local branch main to track the remote branch origin/[branch]. <br>
- After setting this branch, we can directly use <code> git pull </code> and <code> git push </code> <br> 

</ol>

____

<ol>
<h3> <i> File Tracking & Ignoring </i> </h3>

<li> <code> git rm --cached [file_name] </code> </li>
Untracks the file from the Git repository. <br> <br>

<li> <code> git rm [file_name] </code> </li>
Removes the file from the repository. <br> <br>

<li> <code> git mv [existing_file_name] [new_file_name] </code> </li>
Renames the file. <br> <br>

<li> <code> .gitignore </code> </li>
- It is a file created to ignore the folders or files from the Git repository. <br> 
- The format in which the files or folders name written in the .gitignore file is as follows: <br>
folder_name/file_name, /*.extension, /file_name <br> 

</ol>

____

<ol>
<h3> <i> History Navigation & Recovery </i> </h3>

<li> <code> git reflog </code> </li>
- Manages the information recorded in the reference logs, reflogs. <br>
- Reference logs or reflogs are recorded when the tips of the branches and other references were updated in the local repository. <br> <br>

<li> <code> git checkout [commit_id] </code> </li>
- Opens the <i> commit_id </i> as the detached HEAD. <br>
- The detached HEAD means that the HEAD is detatched from the master branch and it is attached to the <i> commit_id </i>. <br>
- Status of the project during that <i> commit_id </i> is retrieved back. <br>
- To go back to the master branch, use <code> git checkout master </code>. <br> 
- Any modifications made in the detatched HEAD does not get saved, which means it does not exists once moved to the master branch. <br> <br>

<li> <code> git checkout --track origin/[branch_name] </code> </li>
Tracks the remotely created and pulled branch. <br> <br>

<li> <code> git show HEAD </code> </li>
Shows detail commit history about the HEAD branch. <br> <br>

<li> <code> git show [commit-id] </code> </li>
Shows detailed commit history for the provided commit-id. <br> <br>

<li> <code> git show HEAD~n </code> </li>
Shows detailed commit history for the nth commit-id. <br> 
E.g. <code> git show HEAD~3 </code> - Shows commit history of the 3rd commit.<br> 

</ol>
