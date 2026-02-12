# Instructions

In this assignment, you will familiarize yourself with two common **version control** workflows using **`git`** and **GitHub**: a **[centralized workflow](#centralized-workflow)**; and a **[forking workflow](#forking-workflow)** (also known as the **"open source workflow"**).

With the centralized workflow, you will set up a **remote** repository on GitHub and a **local** **cloned** **repository** for your own project and practice **pushing** and **pulling** to/from this remote repository.

With the forking workflow, you will contribute to another student's project by **forking** their repository, making changes to your copy, and issuing a **pull request** to them to incorporate your changes.

Performing changes to projects using these two workflows will also allow you to review the archives of the repositories to ensure that your git and GitHub accounts are configured correctly.

Execute the following instructions in order.

## Before you get started

### Disclosure

Note that with version control systems such as `git`, it is easy to verify what work has or has not been done by whom on any project via the [log files](https://knowledge.kitchen/content/courses/software-engineering/slides/git-and-github/#logs). So activity using such systems cannot be faked (not that you would ever consider such a thing)!

### Install Git and create GitHub account

1. Download and install `git` on your local machine, if you haven't already done so.

1. Create an account on [GitHub](https://github.com), if you don't already have one.

## Centralized workflow

In this part, we will try out a simple **centralized workflow**, where developers work with two copies of a repository: a **local** copy, where changes are made; and a **remote** copy, where completed changes are uploaded in order to be backed-up and shared with others.

You will `commit` changes to your local copy and `push` them to your remote copy.

### Create a remote repository on GitHub

Create a new repository on GitHub. If you are viewing this document in your own repository or a repository that has been created for you by your instructor or automatically by **GitHub Classroom**, then this is already done!

### Clone it to your local computer

1.  Clone your remote repository on GitHub to your own local machine.

2.  Create a `README.md` file in that directory using valid Markdown syntax. **Edit** this file such that it includes the following:
    - a link to an article that you find interesting related to software development/engineering (indirect relationships are ok)
    - a paragraph or two about what you find interesting about that article
    - remember that this will be public
    - Use Markdown syntax to make it look nice
3.  **Commit** your `README.md` file to the local repository, including a meaningful commit message.
4.  Open a Terminal window, navigate to your project's main directory, and verify that your changes have been done correctly. Do this by running the command, `git log`.
    - Ensure that every commit shows your correct git username in the `Author` field. We require that your git username be the same as your GitHub username on all commits.
    - Ensure that each commit has only a single line message. We require single-line commit messages and do not accept multiple-line commit messages.
    - If your commits do not meet these requirements, fix the mistakes. Make some small changes to your `README.md` file and try committing again.
    - Do not move forward until you are sure your commits are showing up correctly in the logs according to our requirements.

### Push changes to the upstream remote repository

1.  **Push** the latest version of the files in your local repository to the GitHub repository you created.
1.  Your two repositories should now be in-sync.
1.  Verify this by visiting your remote repository in a web browser and confirming that the `README.md` file there shows all the same changes you made on your own local copy.

### Share your repository with others

1.  Share the link to your GitHub repository on the course's Discord workspace and invite others to collaborate... they will do so via the **forking workflow** outlined below.

## Forking workflow

In this part, we will practice the **forking workflow**, also known as the **open source workflow**. Developers following this type of workflow interact with at least 3 different copies of a repository: the original **remote** repository that the developer wishes to make changes to; a remote **clone** of that official repositor, known as a "`fork`"; and a local clone of the fork.

You will `commit` changes to your local copy of the repository, `push` those changes to your remote fork of the original, and then issue a **Pull Request** from your fork to the original remote repository where you wish your changes to ultimately be incorporated.

### Configure GitHub correctly

In order for Pull Requests on GitHub to be counted as yours, it is necessary that your GitHub username matches exactly your `git` username and that you do not have any other `Name` value in your GitHub Profile.

- Go to your GitHub Profile page in your web browser and remove any `Name` value in your profile. Save any changes.

### Find another repository to work with

1.  Wait for other students to also share their repository links from the centralized workflow part of this assignment.
2.  Select one of the other students' GitHub repository links that you find interesting.

### Fork that repository

1.  **Fork** that repository on GitHub - you now have a clone of that repository in your own GitHub account. We'll refer to this repository as "your forked repository".

### Make a local clone of that fork

1.  **Clone** your forked repository from GitHub to a new directory on your local machine (not the same directory as your original repository). We'll refer to this repository as "your local copy".

### Create a branch

1.  **Create a new branch** of your forked repository on your local copy where, you will make changes to it. Switch to (i.e `checkout`) that branch.
2.  Edit the `README.md` file in your local copy to include a comment from you about that same article mentioned in the file.
    - Make it look well-formatted and written following standard document writing styles, using Markdown syntax.
    - Include your name in the edit you make, so we can clearly see who did it (we can also verify this with the Git logs).
3.  Commit these changes to your local copy, including a meaningful single-line commit message.

### Push changes to your remote fork

1.  **Pull** any changes others may have made to the remote repository on GitHub while you were working.
2.  **Push** your changes to your forked repository on GitHub.
3.  The branch you created with the changes you made will now be updated on your forked repository on GitHub.

### Issue a pull request to the original repository

1.  [Make a pull request](https://help.github.com/articles/creating-a-pull-request/) on the other student's original repository from which you forked yours, asking them politely to include your changes in their original repository

### Accept contributions to your repository

1.  Make sure at least one other student has made a pull request with some changes to your own original repository - use Discord to coordinate this.
2.  If the pull request changes you dislike, leave a response indicating why you have not accepted them, asking the other contributor to fix the problems.
3.  Once you are happy with the changes, accept them.
4.  Pull the updated files to the local repository of your project.
5.  Merge any and all branches to the `main`/`master` branch (whichever is the default in your repository).
6.  Commit any changes, including a meaningful commit message.
7.  Push the result to the remote repository on GitHub.
