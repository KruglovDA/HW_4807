# A quick guide to Git.
## What is Git?
Git is a console utility for tracking and maintaining the history of file changes in your project. With Git-a, you can roll back your project to an older version, compare, analyze, or merge your changes into the repository.
## Basic commands
* **git init** - initializes the local repository.
* **git status** - shows the current state of the git, whether there are changes that need to be committed (saved).
* **git add *file name*** - adds the contents of the working directory to the index (staring area) for a subsequent commit.
* **git commit** - commit or save.
* **git log** - save log.
* **git checkout** - switch between versions.
* **git diff** shows the difference between the current file and the saved one.
## Working with branches
* **git branch** - list of all branches ( * the branch we are on is marked).
* **git branch *branch name*** - create a new branch.
* **git checkout *branch name*** - switch to another branch.
* **git merge *branch name*** - adding a branch to the current one.
* **git branch -d *branch name*** - deleting a branch.
# Syntax of the *Markdown language*
1. **Bold text**
2. *Italic text*
3. ~~Strikethrough text~~
## Download links
1. [VS Code](https://code.visualstudio.com/Download)
2. [Git](https://git-scm.com/)
## Logotypes
![Git logo](logo.png)
![VC Code logo](logo2.png)
## Quotes
>First Citation level
>>Second level of citation
>>>The third level of citation
# Remote repositories
The repository can be: local (located directly in the memory of the developer's computer, development and fixing of changes takes place in it, after which it can be sent to a remote repository) remote (located on the server, can be private – accessible to a limited number of people, and public – open source).
### commands:
* **git clone  *<remote_url>*** - cloning a remote repository to a local machine.
* **git pull** - updating a local branch with changes from a remote repository.
* **git push** - sending local changes to a remote repository
* **git remote** - viewing a list of deleted repositories
* **git remote -v** - подробный просмотр списка удалённых репозиториев с указанием URL.
* **git fetch** - загрузка изменений из удалённого репозитория без слияния с локальной веткой.
* **git branch -r** - просмотр списка удалённых веток.
* **git branch -a** - просмотр списка всех локальных и удалённых веток.
* **git branch --track *<branch_name> <remote_branch>*** - создание локальной ветки, отслеживающей удалённую ветку.
* **git remote add *<remote_name> <remote_url>*** - добавление нового удалённого репозитория.
* **git remote remove *<remote_name>*** - удаление удалённого репозитория.
## How do I set up collaboration?
1. Create an account on GitHub.com .
2. Create a local repository.
3. “Make friends” with your local and remote repositories. 
When creating a new repository, GitHub will tell you how to do it.
4. Send (push) your local repository to a remote one (on GitHub), while
you may need to log in to the remote repository.
5. Make changes “from another computer".
6. Download (pull) the current state from the remote repository.
## pull_request
➜ the team for proposing changes.   
➜ request to inject changes into the repository.
#### How to make a pull request?
1. Making a fork repository (branch).
2. We make the git clone version of the repository OUR OWN.
3. Create a new branch and make our own changes to IT.
4. Commit changes (make commits).
5. We send our version to your GitHub.
6. On the GitHub website, click the pull request button.