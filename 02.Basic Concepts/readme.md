## Basic Concepts ##

### Layman's terms example ###

> Google drive is a file storage/sharing platform
- Imagine you want to share your birthday pictures and videos to a video editor. You can use Google Drive to store and share.
- Take some good Bday Pictures
- create a Google Drive Folder
![Google Drive Folder](https://github.com/yetanothermasterylearning/git/blob/main/02.%20Basic%20Concepts/Pictures/google_drive_folder.png)
- upload your image or video files to Google Drive Folder
- create a sharable link
![Google Drive link](https://github.com/yetanothermasterylearning/Core-Java/blob/main/02.%20Environment%20Setup/Pictures/google_drive_folder_link.png)
- provide access(operations) limits(view or edit option)

>Github is a internet based code hosting platform for version control and collaboration.
- Similar way, you create a project and initialize version control system(here it's git)
- create a GitHub repo (repo is a placeholder/folder)
- upload your project files to GitHub repo
- create a Github(sharable) link
- provide access(operations) permission to edit the files or upload new files

### Types of version control systems? ###
#### Centralized Version Control Systems (CVCS) ####
- a central server that stores the entire codebase and version history. Developers check out files from the central repository, make changes locally, and then commit the changes back to the server. 
- Best suited for projects which run on a Datacenter
- e.g: Concurrent Versions System (CVS), Apache Subversion (SVN).

#### Distributed Version Control Systems (DVCS) ####
- each developer has a complete copy of the codebase, including its full history, on their local machine. This allows for more decentralized and independent development. Developers can commit changes locally and synchronize them with other repositories when needed. 
- e.g: Git, Mercurial.


### Git terminology ###
#### Repository ####
- It's like a folder contains a project's files and meta data like file's version history
#### Local ####
- Repository stored in your computer or any computer
#### Remote ####
- Repository stored in a internet server like github, gitcli or bitbucket
#### Commit ####
- Create a point for file changes. Like a milestone markers on a road.
#### Push and Pull ####
- ![Push and Pull](https://github.com/yetanothermasterylearning/Core-Java/blob/main/02.%20Environment%20Setup/Pictures/push_pull.png)
- Push is a operation to move commit changes from local to remote repository
- Pull is a operation to update commit changes from remote to local repository