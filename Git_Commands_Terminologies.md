2.

[Go to the Git workflow](https://github.com/hkstone14/Team-Project-1/blob/master/Git_workflow.md)

# :point_right: Git commands and terminologies

There are various commands that Git provides but here are some basic git commands mentioned below.

## Repository
* This is a local place/hub on your machine where the entire snapshot of your project is stored. Every minor change is stored and retrievable. Repository logs can easily be viewed and retrieved, i.e, you can jump to any older state of your code.

## Clone
* A clone is a working copy of a remote repository.
* The ‘git clone’ command downloads the remote repository and creates a working directory on your local machine.
* In addition, this command also stores a remote pointer reference from the local repository to the remote repository.
* Command:  ```git clone```

## Fork
* A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.
* Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.
![Image of fork-repo](https://info201-s17.github.io/book/m16-imgs/fork-repo.png)

### Propose changes to someone else's project
1. Fork the repository.
2. Make the fix.
3. Submit a pull request to the project owner.

## Branch
* A branch is a parallel, independent line of development.
* A branch lets you work on the same piece of code in your isolated workspace.
* Every branch has its own copy of the project history and develops on its own code. They are easily and often merged with each other.
* Command: ```git branch <branch-name>```

## Commit
It refers to recording snapshots of the repository at a given time. Committed snapshots will never change unless done explicitly.
![Image of commit](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2016/11/Git-Commit-Workflow-Git-Tutorial-10-Edureka-768x327.png)
* Here, C1 is the initial commit, i.e. the snapshot of the first change from which another snapshot is created with changes named C2. Note that the master points to the latest commit.
* Now, when we commit again, another snapshot C3 is created and now the master points to C3 instead of C2.
* Git aims to keep commits as lightweight as possible. So, it doesn’t blindly copy the entire directory every time you commit; it includes commit as a set of changes, or “delta” from one version of the repository to the other. In easy words, it only copies the changes made in the repository.
* Command: ```git commit```

## Merge
Merging is the way to combine the work of different branches together. This will allow us to branch off, develop a new feature, and then combine it back in.
![Image of Merge](https://wac-cdn.atlassian.com/dam/jcr:86eba9ec-9391-45ea-800a-948cec1f2ed7/Branch-2.png?cdnVersion=kb)
* Command: ```git merge```

## Checkout 
This command switches over to the specified branch and displays the current project state as it is in the branch.
* Command: ```git checkout <brnach-name>```
#### Command
* git checkout feature

when above command will execute,git will switch from current branch to feature branch.It denotes with (*).

## Push
* This command transfer commits from your local repository to your remote repository.
* Pushing exports commits to the remote repositories.
* The use of  git push is to publish your local changes to a central repository. After you’ve accumulated several local commits and are ready to share them with the rest of the team, you can then push them to the central repository by using the following command:
* Command: ```git push <remote>```

## Pull
* The git pull command fetches changes from a remote repository to a local repository. It merges upstream changes in your local repository, which is a common task in Git-based collaborations.
* Pull is reverse of Push command.
* Push exports changes to the remote whereas Pull imports the changes from remote.
* Command: ```git pull origin <branch-name>```
![Image of git push and pull](https://static.javatpoint.com/tutorial/git/images/git-push.png)

## Remote add/remove/show
* git add
 This command adds changes to Git's **Staging Area**, the contents of which can then be wrapped up in a new revision with the "git commit" command.
* git remove
 **git rm** command is used to remove a file from a Git repository.
 Command: ```git rm <file-name>```
* git show
 git show command is used to show objects and objects can be blobs,trees,tags and commit.

## Status
* The **git status** command shows the state of the working directory and the staging area.
* It allows you to see staged changes and the files that aren’t being tracked by Git.
* The git status simply displays what has been going on with **git add** and **git commit** commands.
 ![Image of git status](https://miro.medium.com/max/1668/1*zLxE3Deuc2ePubedcXvlnQ.png)
    
## Master Branch
* A **branch in Git** is simply a lightweight movable pointer to one of these commits. The default **branch** name in **Git** is **master** . As you start making commits, you're given a master branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically
    

    