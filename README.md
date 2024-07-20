# GIT

## Summary:

Git is a widely used decentralized version control system in software development. Here is a summary of key Git concepts:

1. **Repository:**

   * A Git repository is a storage space containing the version history of a project.
   * It can be local on your machine or remote on a server.

2. **Commit:**

   * A commit represents a specific change in the project, accompanied by a descriptive message.
   * It creates a point in the project's history.

3. **Branch:**

   * A branch is an independent line of development that allows working on features or fixes without affecting the main branch (usually called "master" or "main").

4. **Merge:**

   * Merging combines changes from two different branches.
   * It allows incorporating developments made on one branch into another.

5. **Pull Request:**

   * A Pull Request (PR) is a feature of certain Git services, such as GitHub, allowing the submission of changes for review before merging.

6. **Clone:**

   * Cloning a repository means creating a local copy of a remote repository on your machine.

7. **Push:**

   * Pushing means sending local changes to a remote repository.

8. **Pull:**

   * Pulling retrieves changes from a remote repository and integrates them into your local repository.

9. **Status:**

   * The "git status" command displays the status of files in the repository, indicating whether they have been modified, added, or deleted.

10. **Ignoring Files (Gitignore):**

   * A `.gitignore` file specifies files and directories to ignore during Git operations, such as temporary files or configuration files.

In summary, Git is a version control system that allows tracking changes, collaborating on projects, working on independent features via branches, and merging changes in a controlled manner. Basic commands include commit, branch, merge, pull, push, status, and ignore.

## Concepts:
For this projects, we expect you to look at these concepts :
* [Source Code Management](https://intranet.hbtn.io/concepts/878)
* [Git And Github Cheat Sheet](https://intranet.hbtn.io/concepts/879)
* [The Framework](https://intranet.hbtn.io/concepts/880)
* [Approaching A Project](https://intranet.hbtn.io/concepts/881)


# Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General
* What is source code management
* What is Git
* What is GitHub
* What is the difference between Git and GitHub
* How to create a repository
* What is a README
* How to write good READMEs
* How to commit
* How to write helpful commit messages
* How to push code
* How to pull updates
* How to create a branch
* How to merge branches
* How to work as collaborators on a project
* Which files should and which files should not appear in your repo

# Requirements
## General
* A README.md file at the root of the repo, containing a description of the repository
* A README.md file, at the root of the folder of this project (i.e. git), describing what this project is about
* Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
* Your answer files should only contain the command, and nothing else

# More Info
## Install git
### If git is not already installed on your terminal:

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

# Basic usage
## At the end of this project you should be able to reproduce and understand these command lines:

```bash
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main 
```
