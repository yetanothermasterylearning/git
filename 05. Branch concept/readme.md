## Git Branch Concept ##
- What is a branch?
- Why we need a branch?
- Creating branches locally
- Checkout a branch
- Merging a branch
- Delete a branch
- Branch naming standard approach
- Assignment

#### What is a branch? ####
- Git Branches help us work on different parts of the project.
- In technical terms, Branch is a lightweight movable pointer pointing to a specific version history commit. When you create a new branch, it effectively creates a new line of development, allowing you to work on a particular feature or bug fix independently from the main line of development
- In Layman's terms, Imagine you and your friend share a two-bedroom apartment. Each of you has your own bedroom for sleeping or working without disturbing the other. You can watch TV together in the living space. Similarly, developers can independently create their branch and work on it. Once the work completes, they can merge all the changes into the main/master branch and provide the whole project.

### Layman's terms example ###
- Imagine you are conducting a birthday party for your kid at a park. 
- You plan to decorate a stage, bring a cake, and arrange excellent food. 
- You got a fantastic idea that you can share the work with friends. Assume You can work on decorating the stage and request friend "A" to collect the cake and friend "B" to collect the food. 
- Each person works independently and finishes the party. 
![branch example](https://github.com/yetanothermasterylearning/git/blob/main/05.%20Branch%20Concept/Pictures/branch_example.png)
- Similar way, you create a project plan with the required features
- Allocate the work to developers
- Individual developers can work independently by creating an individual branch
- At the end, you can merge all changes to a master/main branch(the code)
![branch example](https://github.com/yetanothermasterylearning/git/blob/main/05.%20Branch%20Concept/Pictures/git_branch_example.png)

#### Why we need a branch? ####
- Branches allow multiple people to work on the same project at the same time without interfering with each other's work.
- Branches help us to work independently, quick roll back, experimentation with out disturbing the original code, parallel collabration and versioning.

#### Creating a branch in local ####
- Open a terminal or command prompt in the directory where your Git repository is located.
- use ```git branch <new_branchname>``` to create a branch

#### Checkout a branch in local ####
- Open a terminal or command prompt in the directory where your Git repository is located.
- use ```git checkout <existing_branchname>``` to checkout an existing branch

#### Creating branch and checkout in local ####
- Open a terminal or command prompt in the directory where your Git repository is located.
- use ```git checkout -b <new_branchname>``` to checkout to a new branch

#### display all branches in local ####
- Open a terminal or command prompt in the directory where your Git repository is located.
- use ```git branch``` to list all branches

#### Delete a branch in local ####
- Open a terminal or command prompt in the directory where your Git repository is located.
- Swith to another branch using checkout command. You can delete the checkedout branch.
- If the branch you want to delete has no unmerged changes (you've already merged those changes into another branch), you can use the -d option to delete it.
	- use ```git branch -d <branchname>``` to delete a branch
- If you want to forcefully delete the branch regardless of unmerged changes, you can use the -D option:
	- use ```git branch -D <branchname>``` to delete a branch forcefully

#### Merging a branch ####

#### Branch naming standard approach ####

### Assignment ###
#### Assignment-1 ####

#### Assignment-2 ####

#### Crazy thought :wink: ####

