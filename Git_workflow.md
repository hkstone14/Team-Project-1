 3.

[go to Docker Usage](https://github.com/hkstone14/Team-Project-1/blob/master/Docker_usage.md)

# Git workflow

## Initialize the central repository
First, someone needs to create the central repository on a server. If it’s a new project, you can initialize an empty repository. Otherwise, you’ll need to import an existing Git repository.

## Hosted Central Repository
* Central repositories are often created through 3rd party Git hosting services like Github,Bitbucket. 
* The process of initializing a bare repository discussed above is handled for you by the hosting service. 
* The hosting service will then provide an address for the central repository to access from your local repository.

## Clone Central Repository
* Next, each developer creates a local copy of the entire project. This is accomplished via the **git clone** command.
* When you clone a repository, Git automatically adds a shortcut called origin that points back to the “parent” repository, under the assumption that you'll want to interact with it further on down the road. 

## Make changes and commit
Once the repository is cloned locally, a developer can make changes using the standard Git commit process: edit, stage, and commit. If you’re not familiar with the staging area, it’s a way to prepare a commit without having to include every change in the working directory. This lets you create highly focused commits, even if you’ve made a lot of local changes.

## Push new commits to the central repository
* Once the repository is cloned locally, a developer can make changes using the standard Git commit process: edit, stage, and commit. If you’re not familiar with the staging area, it’s a way to prepare a commit without having to include every change in the working directory. This lets you create highly focused commits, even if you’ve made a lot of local changes
Example: git push origin master
* This command will push the new committed changes to the central repository. When pushing changes to the central repository, it is possible that updates from another developer have been previously pushed that contain code which conflict with the intended push updates. Git will output a message indicating this conflict.

## Managing conflicts
The central repository represents the official project, so its commit history should be treated as sacred and immutable. If a developer’s local commits diverge from the central repository, Git will refuse to push their changes because this would overwrite official commits.

![Image of Git workflow](https://miro.medium.com/max/2800/1*9yJY7fyscWFUVRqnx0BM6A.png)