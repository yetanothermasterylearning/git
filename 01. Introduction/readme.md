## Version control systems (VCS) Introduction ##

### What is a Version Control System? ###
- The Version control systems (VCS) are software tools that help manage changes to a set of files or a collection of code, enabling multiple people to collaborate on a project. 
- They track the history of modifications made to files, allowing users to easily revert to previous versions, compare changes, and merge modifications from different sources.
- The primary purpose of a version control system is to keep a historical record of changes made to a project's files or source code. 
- It allows developers to work on different features or bug fixes concurrently without directly affecting each other's work.
![Version Control System](https://github.com/yetanothermasterylearning/git/blob/main/01.%20Introduction/Pictures/version_control_system.png)

### Why do we need a Version Control System? ###
- Just as we store digital pictures, emails, and resumes in file format, we also store software components such as code files for Java, C, C++, and Python, infrastructure elements like ARM templates, Terraform, and Cloudformation, and configuration files in formats like XML and YAML. To manage changes to these files, a system is necessary.
![Version Control System](https://github.com/yetanothermasterylearning/git/blob/main/01.%20Introduction/Pictures/version_control_system_2.png)

### What are the different version control systems? ###
- Centralized Version Control Systems (CVCS): a central server that stores the entire codebase and version history. Developers check out files from the central repository, make changes locally, and then commit the changes back to the server. 
- e.g: Concurrent Versions System (CVS), Apache Subversion (SVN).
![Centralized Version Control Systems](https://github.com/yetanothermasterylearning/git/blob/main/01.%20Introduction/Pictures/cvcs.png)

- Distributed Version Control Systems (DVCS): each developer has a complete copy of the codebase, including its full history, on their local machine. This allows for more decentralized and independent development. Developers can commit changes locally and synchronize them with other repositories when needed. 
- e.g: Git, Mercurial.
![Version Control System](https://github.com/yetanothermasterylearning/git/blob/main/01.%20Introduction/Pictures/version_control_system_2.png)
- ![Distributed Version Control Systems](https://github.com/yetanothermasterylearning/git/blob/main/01.%20Introduction/Pictures/dvcs.png)

### What is Git? ###
- As metnioned previously, [Git](https://en.wikipedia.org/wiki/Git) is a Distributed Version Control System. Git was originally authored by Linus Torvalds. 
- It become the most widely used version control system due to its distributed nature, speed, and powerful features.