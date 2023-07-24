## Git Project Flow ##
- Creating Git and GitHub repository - end to end example
    - local repository
    - remote repository
    - Push the local changes to remote using Git command line interface
    - (Optional) Push the local changes to remote using sourcetree tool (GUI)
- File states
    - Untracked
    - Tracked/Staged
    - Modified
    - Committed
- Git basic commands
    - git init
    - git status
    - git add
    - git commit
    - git push
- Git ignore file

### Creating Git and GitHub repository - end to end example ###
- Assume you want to start a startup. You want to track your programming project file changes using ***Git*** on local computer, and your future goal is to hire more developers and collaborate on the project with them using ***GitHub***.
- You will learn the first phase steps and concepts in this chapter; and How multiple developers can work simultaneously on a project in the next chapter.

#### local repository ####
> Tracking your programming project file changes using ***Git*** on local computer
- Create a director with name **firstproject**
- Navigate to **firstproject** director and create a sample **README.txt** file.
> If you are familiar with any programming language, please create a programming file like HelloWorld.java or HelloWorld.py, or HelloWorld.c file.
- type any sample test in the file.
- Open terminal(command tool in Windows) and Navigate to the **firstproject** director using `cd` command
- type `git init`
> git init is a command initializing a new or empty directory as a Git repository like instructing git to monitor any modifications made to files in the present directory.
- git maintain 4 stages of File changes
    - Untracked: When you create a new file to your project directory, Git considers it untracked until you explicitly tell Git to start tracking it by using init command.
    - Modified: After you make changes to a tracked file, Git recognizes that the file has been modified since the last commit. These changes are not yet committed.
    - Staged: After you make changes to a tracked file, can move the file changes to interim state befire commit. Git recognizes that the file has been modified and ready for the next commit.
    - Committed: Once you run git commit, the changes to the tracked files in the staging area are permanently saved in the Git repository as a new commit.
> let's see all stages for the **README.txt** file.
- type `git status` and press enter. Git status command provide the all file status. It shows the README.txt file is a Untracked file.
- type `git add README.txt` and press enter. Git add command move the file from Untracked to Tracked.
- type `git status` and press enter. This time git status shows **README.txt** file changes to be committed.
- type `git commit -m "Initial commit"` and press enter. The changes to the tracked files in the staging area are permanently saved in the Git repository as a new commit.
> -m option to provide the commit message.
![local repository](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/local_repository.png)

#### remote repository ####
> Creating ***GitHub*** account
- Go to [github](https://github.com/) and signup for your account. [Ref: GitHub account creation steps](https://github.com/yetanothermasterylearning/git/tree/main/03.%20Environment%20Setup#create-github-account).
- Login to [github](https://github.com/). It will open a dashboard page
![github_dashboard](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/github_dashboard.png)
- Click new button to creat a repository. Give repository name same as your local project(e.g: firstproject) and keep other options as default
![git_repository_creation](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/git_repository_creation.png)
- Copy the reposiotry ssh link
![git_repository_link](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/git_repository_link.png)<br/>

#### Push the local changes to remote using Git command line interface ####
> Push your project changes to ***GitHub*** and collaborate it with others
- Go to terminal(command tool in Windows) and Navigate to the **firstproject** director using `cd` command
- type `git remote add origin <url>` and press enter.
- type `git push -u origin master` and press enter.
![git_push_to_remote](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/git_push_to_remote.png)
- Refresh the Github project page.
![github_firstproject](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/github_firstproject.png)

#### Push the local changes to remote using Sourcetree tool ####
> Push your project changes to ***GitHub*** and collaborate it with others
- Open Sourcetree tool and click New -> Add Existing Local Repository
![sourcetree_add](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_add.png)
- Select **firstproject** director, it add **firstproject** repository to home screen
![sourcetree_dashboard](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_dashboard.png)
- double click the **firstproject** repository on home screen, it will open the GUI for the repository changes.
![sourcetree_firstproject](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_firstproject.png)
- Open "README.txt" and add some test in the file.
- after saving file, sourcetree file changes screen(rightside widget) display all uncommented/modified changes.
![sourcetree_uncommited](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_uncommited.png)
- Like git command interface way, we need to apply add and commit commands from sourcetree.
- On sourcetree, click file changes and split the view between staged and unstaged files
![sourcetree_splitview](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_splitview.png)
- Select unstaged **README.txt** file. It will move the recent changes to staged area. It's nothing but `git add` command.
- Add commit message and click commit button.
![sourcetree_commit](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_commit.png)
- After successful commit operation, the push button higheligh with number of commits(Here it's one) which are ready to push to master.
![sourcetree_ready_push](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_ready_push.png)
- Click repository setting to configure remote. We have already configured the remote in the previous section. It's nothing but `git remote add origin <url>` command.
![sourcetree_repo_settings](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_repo_settings.png)
![sourcetree_repo_settings_remote](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_repo_settings_remote.png)
- Go to sourcetree screen and click push button. Open a remote branch details and click push button
![sourcetree_push](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/sourcetree_push.png)
- Refresh the Github project page.
![github_firstproject_2](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/github_firstproject_2.png)

(`***`)
> You can invite others to collabrate this project by addeding collaborators in this repository setting.
![github_collaborators](https://github.com/yetanothermasterylearning/git/blob/main/04.%20Git%20Project%20Flow/Pictures/github_collaborators.png)<br/>
(`***`)

### File states ###
- git maintain 4 stages of File changes
    - Untracked: When you create a new file to your project directory, Git considers it untracked until you explicitly tell Git to start tracking it by using init command.
    - Modified: After you make changes to a tracked file, Git recognizes that the file has been modified since the last commit. These changes are not yet committed.
    - Staged: After you make changes to a tracked file, can move the file changes to interim state befire commit. Git recognizes that the file has been modified and ready for the next commit.
    - Committed: Once you run git commit, the changes to the tracked files in the staging area are permanently saved in the Git repository as a new commit.

### Git basic commands ###
- git init
- git status
- git add
- git commit
- git push

### Git ignore file ###
