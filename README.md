# GithubCLI
Git hub commands step-by-step for beginers - hotfix

Install Git
- Windows: https://git-scm.com/download/win

Refer following,
- popular online book at https://git-scm.com/book/en/v2
- Visual studio Code, Git integration at https://code.visualstudio.com/docs/editor/versioncontrol

Git commands
- https://git-scm.com/docs

Basic branching and merging
- https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

# Configuring and connecting to a remote repository
Reference: https://www.computerhope.com/issues/ch001927.htm

- Move to the project directory root

- Type the following command to configure your Git username, where "your name" will be your GitHub username.

	$ git config --global user.name "your name"

- After entering the above command, you should be returned to the command prompt. Next, enter your e-mail address by typing the following command, where "your e-mail" is your e-mail address.

	$ git config --global user.email "your e-mail"

- Once the above steps have been completed, you'll be ready to connect to a remote repository. To find the repository address, go to a repository on GitHub and click the Clone or download repository link to get the address. For example, we've created a repository called "GithubCLI" at https://github.com/ArohanGit/GithubCLI.git address. Copy the address to your clipboard.

- Once copied go back to the command line and type the following command, where URL is the address you copied. To paste that address into the command line right-click in the command line window and click paste.

	**$ git clone "remote repository URL"**

- Once the Git repository is created local clone, you'll have a new directory in your current directory with the name of the Git repository.

- Once the Git remote repository is cloned to your local repository, you should have a new folder in the current directory with the name of the Git repository. For example, in our "GithubCLI" Git we would have a new directory called "GithubCLI"". Use the cd command to change into the new directory.

- Once in the new directory, type the following command to list the remote repositories.

	$ git remote

- If successful, you should see "origin" that is the name of your master Git branch. To see the aliases (URL or path), type the following command.

	$ git remote -v


# Adding an existing project to github repo using CLI
Reference:  https://help.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line

- Initialises the git for the project root

	**$ git init**

- Adds the remote repo origin

	**$ git remote add origin "remote repository URL"**

- Verifies the new remote URL

	**$ git remote -v**

- Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

	**$ git add .**

- Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify   the file, use 'git reset --soft HEAD~1' and commit and add the file again.

	**$ git commit -m "First commit"**

- Pushes the changes in your local repository up to the remote repository you specified as the origin

	**$ git push origin master**

- **Other useful commands**

	$ git config --list
    
	$ git config user.name
