# GithubCLI
Git hub commands step-by-step for beginers

# Step 1 Configuring and connecting to a remote repository
Reference: https://www.computerhope.com/issues/ch001927.htm

# --1
# move to the project directory root

# --2 
# Type the following command to configure your Git username, where <your name> will be your GitHub username.

$ git config --global user.name "<your name>"

# --3
# After entering the above command, you should be returned to the command prompt. Next, enter your e-mail address by typing the following command, where <your e-mail> is your e-mail address.

$ git config --global user.email "<your e-mail>"

# --4
# Once the above steps have been completed, you'll be ready to connect to a remote repository. To find the repository address, go to a repository on GitHub and click the Clone or download repository link to get the address. For example, we've created a repository called "example" at https://github.com/ArohanGit/GithubCLI.git address. Copy the address to your clipboard.

# --5
# Once copied go back to the command line and type the following command, where <URL> is the address you copied. To paste that address into the command line right-click in the command line window and click paste.

$ git clone <URL>

# --6
# Once the Git repository is created local clone, you'll have a new directory in your current directory with the name of the Git repository.

# -- 7
# Once the Git remote repository is cloned to your local repository, you should have a new folder in the current directory with the name of the Git repository. For example, in our "GITHUBCLI" Git we would have a new directory called "GITHUBCLI". Use the cd command to change into the new directory.

# --8
# Once in the new directory, type the following command to list the remote repositories.

$ git remote

# --9
# If successful, you should see "origin" that is the name of your master Git branch. To see the aliases (URL or path), type the following command.

$ git remote -v


# Step 2
Adding an esisting project to github repo using CLI

https://help.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line


$ git init
# Initialises the git for the project root

$ git remote add origin <remote repository URL>
# Adds the remote repo origin

$ git remote -v
# Verifies the new remote URL

$ git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.

$ git remote add origin remote repository URL
# Sets the new remote

$ git remote -v
# Verifies the new remote URL

$ git push origin master
# Pushes the changes in your local repository up to the remote repository you specified as the origin

# Other useful commands
$ git config --list
$ git config user.name

