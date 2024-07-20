# GIT

## Summary:

## GIT

Git is a version control system that allows tracking changes in a project. Commits record snapshots of the code, branches enable parallel development, and merges incorporate changes. Pull Requests facilitate collaboration by allowing review before merging. Cloning creates a local copy, pushing sends commits to a remote repository, and pulling retrieves changes. The "git status" command provides the file status, and the .gitignore file specifies files to ignore. In summary, Git offers precise control over project evolution, promotes collaboration, and enables efficient version management.

## GITHUB

GitHub is a collaborative development platform based on Git, offering advanced features for storage, management, and collaboration around Git repositories.

1. Repositories:

GitHub hosts Git repositories, which are storage spaces for projects containing version history and associated files.

2. Collaboration:

Facilitates collaboration among developers by allowing repository sharing, Pull Requests for code review, and discussions about changes.

3. Project Management:

Offers project management features with Kanban boards, issues, and projects, making it easy to track tasks and issues.

4. Continuous Integration:

Supports continuous integration with services like GitHub Actions, enabling automation of tests and deployments.

5. Hosting Pages:

Allows hosting static websites directly from repositories using the GitHub Pages service.

6. Social Network:

GitHub functions as a social network for developers, making it easy to discover projects, follow other developers, and participate in open source communities.

In summary, GitHub is a comprehensive platform that simplifies Git project management, encourages collaboration among developers, provides advanced project management tools, and operates as a social community for development enthusiasts.

## GIT and GITHUB

Using Git and GitHub involves several steps, from initial configuration to daily project management. Here is a general guide:

### Initial Configuration:
1. Install Git:

* Download and install Git from git-scm.com.
* Configure your username and email using the command:
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

2. Create a GitHub account:

* Go to GitHub and create an account.

3. Generate an SSH key pair (optional but recommended):

* Follow instructions here to generate SSH keys.

### Create a New Repository:
1. Initialize a local repository:

* Use the git init command in your project directory.
2. Add files to Git tracking:

* Use git add to add files to Git tracking.
```bash
git add file1 file2
```

3. Make a commit:

* Save changes with a commit.
```bash
git commit -m "Descriptive message"
```

### Working with Branches:
1. Create a new branch:

* Use git branch to create a new branch.
```bash
git branch branch_name
```

2. Switch between branches:

* Use git checkout to switch branches.
```bash
git checkout branch_name
```

3. Merge branches:

* Merge a branch using git merge.
```bash
git merge branch_name
```

### Working with GitHub:
1. Create a repository on GitHub:

* On GitHub, create a new repository.

2. Link the local repository to GitHub:

* Add the remote repository with git remote.
```bash
git remote add origin link_to_your_github_repo.git
```

3. Push commits to GitHub:

* Use git push to send your commits to GitHub.
```bash
git push -u origin your_branch_name
```

4. Create a Pull Request (PR):

* On GitHub, create a PR to request the merging of your changes.

5. Fetch changes from GitHub:

* Use git pull to retrieve changes from GitHub.
```bash
git pull origin your_branch_name
```

## Resources:
* [Resources To Learn Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
* [Git And Github Cheat Sheet](https://intranet.hbtn.io/concepts/879)
* [The Framework](https://intranet.hbtn.io/concepts/880)
* [Approaching A Project](https://intranet.hbtn.io/concepts/881)

## Requirements:

* A README.md file at the root of the repo, containing a description of the repository
* A README.md file, at the root of the folder of this project (i.e. git), describing what this project is about
* Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
* Your answer files should only contain the command, and nothing else

## More Info

### Install git

If git is not already installed on your terminal:

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

### Basic usage

At the end of this project you should be able to reproduce and understand these command lines:

```bash
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```
## TASKS: 

### 0. Create And Setup Your Git And Github Account
#### Step 0 - Create an account on GitHub

You will need a GitHub account for all your projects. You can create an account for free here

#### Step 1 - Create a Personal Access Token on Github

To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow this tutorial to create a token.

#### Step 2 - Update your profile on the Intranet

Update your Intranet profile by adding your Github username here

If it’s not done the Checker won’t be able to correct your work

#### Step 3 - Create your first repository

Using the graphic interface on the github website, create your first repository.

* Name: Look at the bottom of the project to see the name of the repository
* Description: This is my first repository as a full-stack engineer
* Public repo
* No README, .gitignore, or license

#### Step 4 - Open the sandbox

On the intranet, just under the task, click on the button >_Get a sandbox and run to start the machine. Once the container is started, click on >_Webterm to open a shell where you can start work from.

#### Step 5 - Clone your repository

On the webterm of the sandbox, do the following:

* Clone your repository

```bash
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository.
```

* Replace {YOUR_PERSONAL_TOKEN} with your token from step 1
* Replace {YOUR_USERNAME} with your username from step 0 and 1
* Replace {YOUR_REPO} with the name of the reposotiry at the bottom of the task

#### Step 6 - Create the README.md and push the modifications

* Navigate to this new directory. Tips

```bash
root@896cf839cf9a:/# cd {YOUR_REPO}/
root@896cf839cf9a:/{YOUR_REPO}#
```

* Create the file README.md with the content My first readme. Tips

```bash
root@896cf839cf9a:/{YOUR_REPO}# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/{YOUR_REPO}# cat README.md                                                                                      
My first readme                                                                                                                       
```                                                                                                         
* Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin

```bash
root@896cf839cf9a:/{YOUR_REPO}# git add .
root@896cf839cf9a:/{YOUR_REPO}# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/{YOUR_REPO}# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                                                                                       
 * [new branch]      master -> master 
```

Good job!

You pushed your first file in your first repository.
You can now check your repository on GitHub to see if everything is good.

### 1. Repo-Session
Create a new directory called git in your repo.
Make sure you include a not empty README.md in your directory:

* at the root of your repository
* AND in the directory git

And important part: Make sure your commit and push your code to Github - otherwise the Checker will always fail.

### 2. Coding Fury Road
For the moment we have an empty project directory containing only a README.md. It’s time to code !

* Create these directories at the root of your project: bash, c, js
* Create these empty files:
 * c/c_is_fun.c
 * js/main.js
 * js/index.js

* Create a file bash/best with these two lines inside: #!/bin/bash and echo "Best"
* Create a file bash/school with these two lines inside: #!/bin/bash and echo "School"
* Add all these new files to git
* Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

3. Collaboration Is The Base Of a Company
A branch is like a copy of your project. It’s used mainly for:

* adding a feature in development
* collaborating on the same project with other developers
* not breaking your entire repository
* not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch update_script and in this branch:

* Create an empty file named bash/98
* Update bash/best by replacing echo "Best" with echo "Best School"
* Update bash/school by replacing echo "School" with echo "The school is open!"
* Add and commit these changes (message: “My personal work”)
* Push this new branch Tips

Perfect! You did an amazing update in your project and it’s isolated correctly from the main branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

* Change branch to main
* Update the file bash/best by replacing echo "Best" with echo "This School is so cool!"
* Delete the directory js
* Commit your changes (message: “Hot fix”) and push to the origin

### 4. Collaboration: Be Up To Date
Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – and only for this task – please update your file README.md in the main branch from GitHub.com. It’s the only time you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

* Get all changes of the main branch locally (i.e. your README.md file will be updated)
* Create a new file up_to_date at the root of your directory and in it, write the git command line used
* Add up_to_date to git, commit (message: “How to be up to date in git”), and push to the origin

### 5. Haaa What Did You Do ???
Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch update_script to main: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

HHHHHHHAAAAAAAA

```bash
CONFLICT (content): Merge conflict in bash/best
```


As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch update_script, and push the result to the origin.

At the end, you should have all your work from the branch update_script (new file and two updated files) and all latest main commits (new files, delete folder, etc.), without conflicts.

### 6. Never Push Too Much
Create a .gitignore file and define a rule to never push ~ files (generated by Emacs). Tips
