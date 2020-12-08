# Notes Git Course

## Git configuration
Starting A Project

`$ git config --global user.name “Your Name” `

Set the name that will be attached to your commits and tags.

`$ git config --global user.email “you@example.com”`

Set the e-mail address that will be attached to your commits and tags.

`$ git config --global color.ui auto`

Enable some colorization of Git output.


## Concept: Three States of Git

Git has three main states that your files can reside in:

- Committed
- Modified
- Staged

**Committed**
This state indicates that the file is safely stored in the local database.

**Modified**
When any change to the file occurs, the state of the file changes from committed to modified

**Staged**
When we're finished with all the modifications to our file, it moves to the staged state. The file is now ready to be added to the local git database, you have marked it to go into your next commit snapshot.

## Concept: Three Sections of a Git Project
Similar to how files can be in three different states, a Git project consists of three different sections.

**.git directory**
The first section is the .git directory, also known as the repository. This is where Git stores the metadata and object database for your project.

**working directory**
The next section is the working directory. This is a single checkout of one version of the project. This is where you can modify files.

**staging area**
The third section is the staging area, also known as the index. It's the area between the working directory and the .git directory. All the files which are ready for a commit are stored here.

When we commit, what is in the staging area moves to the new version of the repository. This excludes what is in the working directory. This allows us to change files however we like, but only what we move to the staging area will be committed. Everything we changed but do not want to put in a repository stays in the working directory.



## Starting A Project

`$ git config --global user.name “Your Name”`

Set the name that will be attached to your commits and tags.

`$ git config --global user.email “you@example.com”`

Set the e-mail address that will be attached to your commits and tags.

`$ git config --global color.ui auto`

Enable some colorization of Git output.

`$ git init [project name]`

Create a new local repository. If [project name] is provided, Git will
create a new directory name [project name] and will initialize a
repository inside it. If [project name] is not provided, then a new
repository is initialized in the current directory.

`$ git clone [project url]`

Downloads a project with the entire history from the remote repository

## Day-To-Day Work

`$ git status`

Displays the status of your working directory. Options include new,
staged, and modified files. It will retrieve branch name, current commit
identifier, and changes pending commit.

`$ git add [file]`

Add a file to the staging area. Use in place of the full file path to add all
changed files from the current directory down into the directory tree.

`$ git diff [file]`

Show changes between working directory and staging area.

`$ git diff --staged [file]`

Shows any changes between the staging area and the repository.

`$ git checkout -- [file]`

Discard changes in working directory. This operation is unrecoverable.

`$ git reset [file]`

Revert your repository to a previous known working state.

`$ git commit`

Create a new commit from changes added to the staging area.
The commit must have a message!

`$ git rm [file]`

Remove file from working directory and staging area.

`$ git stash`

Put current changes in your working directory into stash for later use.

`$ git stash pop`

Apply stored stash content into working directory, and clear stash.

`$ git stash drop`

Delete a specific stash from all your previous stashes

## Review your work

Review your work

`$ git log [-n count]`

List commit history of current branch. -n count limits list to last n
commits.

`$ git log --oneline --graph --decorate`

An overview with reference labels and history graph. One commit
per line.

`$ git log ref..`

List commits that are present on the current branch and not merged
into ref. A ref can be a branch name or a tag name.

`$ git log ..ref`

List commit that are present on ref and not merged into current
branch.

`$ git reflog`

List operations (e.g. checkouts or commits) made on local repository