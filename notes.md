## 📒 Git – Notes

> 🗓️ Last Updated: 2025-08-06 <br>
> 🏷️ Part of my Week 2 of #CodetoCareer journey

---

## 1. Introduction

- Git is an open-source distributed version control system. <br>
- Created by <i>Linus Torvalds</i> <br>
- Allows multiple developers to collaborate on the project. <br>
- No risk of overwritting of the work by fellow developers. <br>

---

## 2. Why Use Git?

- Collaboration <br>
- History Tracking <br>
- Branching and Merging <br>
- Distributed Development <br>

---

<blockquote><b>Notes:</b><br>
Local Repository - Project version is stored in the computer <br>
Remote Repository - Project version is stored on a server accessible to other <br>
Server - Computer program that provides services to other computers, over a network
</blockquote>

---

## 3. Core Concepts

<ol>
<li> Repositories (repo) </li>
- Storage place for projects code base and history <br>
- Two types of repositories: Local and Remote <br> 

<br>

<li> Commits </li>
- Snapshot of the project at a specific time <br>
- Saves changes made to the project <br>
- Each commit has a unique identifier (<i> also known as hash</i>, which is a 40 digit SHA-1 key) and a commit message (description of the changes made) <br>
- Allows to track the changes and helps in reviewing the code <br>

<br>

<li> Branches </li>
- Separate line of development for bug fixes and feature development <br>
- Main branch created while initialisation of the git repo is the default branch <br>
- Branches can be merged back to the main branch <br>

<br>

<li> Merging </li>
Process of integrating one branch into another is known as merging. <br>

<br>

<li> Cloning </li>
- Creating a copy of remote repo in the local system i.e. creating a local repo from the remote repo <br>
- Copy contains files of the codebase, branches and commit history <br>

<br>

<li> Pull </li>
Asking for contents or changes from remote repo to the local repo <br>

<br>

<li> Push </li>
Asking for contents or changes from local repo to the remote repo <br>

<br>
</ol>

---

## 4. Git Workflow

There are 3 areas in the Git workflow: 

<ol>
<li> Working Directory </li>
- Place where files are created, modified, updated and deleted <br>
- Changes made in the working directory are not saved unless the changes are staged <br>

<br>

<li> Staging Area </li>
- Changes made in the working directory are staged here <br>
- Staged means the changes are saved and they are ready to be committed <br>
- Also known as the index of the git repository <br>

<br>

<li> Repository </li>
- The files in the staging area are saved in the repository <br>

<br>
</ol>

<img src = "https://github.com/ashweeni-b/Git-Notes/blob/main/assets/Git%20Workflow.jpg" alt = "Change directory to D drive" width = "400" />

---

## 5. Different file states in Git

<ol>
<li> Untracked files </li>
Files within the working directory which Git is not managing <br> <br>

<li> Tracked files </li>
Files within the working directory and managed by Git <br> <br>

<li> Unmodified files </li>
Files with no changes or modifications <br> <br>

<li> Modified files </li>
Files with changes or modifications <br> <br>

<li> Unstaged files </li>
Modified files which are not ready to commit <br> <br>

<li> Staged files </li>
Modified files which are ready to commit <br> <br>

</ol>

---
## 6. Git Installation 

Refer [How to install Git on Windows 11](https://youtu.be/t2-l3WvWvqg?si=LcF-lqIZFgKzTAL5) by Amit Thinks

---

## 7. Git Commands

Refer [commands.md](./commands.md) for list of commands and their use.

---


## 8. Questions

1. 

---


## 9. References

- [Git - Introduction](https://www.geeksforgeeks.org/git/git-introduction/)
- [How to Install Git on Windows Command Line?](https://www.geeksforgeeks.org/installation-guide/how-to-install-git-on-windows-command-line/)
- [How to install Git on Windows 11](https://youtu.be/t2-l3WvWvqg?si=LcF-lqIZFgKzTAL5)
- [CodetoCareer - Week 2](https://www.linkedin.com/posts/activity-7350177852027232256-h1JE?utm_source=share&utm_medium=member_desktop&rcm=ACoAAE-UhZwBDTW7JxUFdBcAbzubFz_HhQRI1Ng)
