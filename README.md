
# Git and Github

Let’s start with the basics. Git is a version control system that allows you to track changes to your files and collaborate with others. It is used to manage the history of your code and to merge changes from different branches. I can understand that as of now these terms like version control, branches, and merges are not familiar to you. But don’t worry, we will learn them in this tutorial.

# What is Git

Git is like the superhero of version control systems, swooping in to save the day for developers everywhere. Created by the legendary Linus Torvalds in 2005 and now looked after by the awesome Junio Hamano, Git is the go-to tool for tracking code changes, keeping tabs on who did what, and making coding collaboration a breeze.

### So, what does this superhero (GIT) do?

manages projects with repositories, which are like secret hideouts for your code. You can clone a project to work on your own local copy, control and track changes with fancy features like staging and committing, branch out to work on different parts of a project, merge everything back together seamlessly, pull the latest updates, and push your own changes like a boss. 



#### It is used for:

-  Tracking code changes
- Tracking who made changes
- Coding collaboration

# Working with Git
1. **Initialize Git** : This is where the magic begins. You turn a regular folder into a Git repository, and voila, Git starts keeping track of every little change.

2. **Track Changes** : Git is like your coding buddy who never forgets anything. It knows when a file is changed, added, or deleted, and keeps a watchful eye on everything.

3. **Stage and Commit** : Think of staging as picking out your favorite toys to play with. You select the changes you want to keep, and then commit them, creating a permanent snapshot that Git will never let go of.

4. **Time Travel** : Yes, you heard it right. With Git, you can travel back in time! Okay, maybe not literally, but you can revert to any previous version of your project with ease.
# why Git
- **Popularity** : Over 70% of developers swear by Git. Need we say more?

- **Global Collaboration** : With Git, developers from every corner of the globe can work together seamlessly. Distance is no match for Git-powered teamwork.

- **Full Project History** : Git keeps track of every twist and turn in your project's journey. No more lost changes or forgotten updates.

- **Undo Button** : Made a mistake? No worries! Git lets you roll back to a previous version faster than you can say **"commit"** .
## what about GitHub?
GitHub isn't Git, but it's like its trusty sidekick. It takes Git to the next level with a whole suite of tools and features. Owned by the mighty Microsoft, GitHub is the ultimate hub for all things code, hosting millions of repositories from developers worldwide.

So, there you have it! Get ready to dive into the exciting world of Git and GitHub, where coding dreams become reality.
## What is Repository.
In the world of programming and software development, a repository is an essential tool that serves as a central location for storing and managing code. It not only houses the source code but also tracks changes, manages versions, and facilitates collaboration among developers. Let's delve into the intricacies of what a repository is and why it's indispensable in modern software development.


# Git Install in Your System

Setting up Git in your system for use with Visual Studio Code is essential for efficient version control and collaboration. Here's a straightforward guide to help you get started.

### Step-by-Step Instructions

1. Install Git
- **Windows** : Download and install from Git for [Windows](https://www.git-scm.com/).
- **Mac** : Use Homebrew with brew install git or download from Git for [Mac](https://git-scm.com/download/mac).
- **Linux** : Install via package manager, e.g., `sudo apt-get install git` for Debian-based distributions.

2. Verify Git Installation
Open your terminal or command prompt and run:
```cmd
  git --version
```
You should see the installed Git version.
This command will display the version of git installed on your system. Git is a very stable software and don’t get any breaking changes in majority of the cases, at least in my experience.

3. Configure Git
Set up your username and email:
```cmd
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
```
Check your configuration with:

```cmd
  git config --list
```
4. Install Visual Studio Code
Download and install from [Visual Studio Code](https://code.visualstudio.com/).

5. Install Git Extension in VS Code
Open VS Code.
Go to the Extensions view by clicking the Extensions icon in the Activity Bar on the side of the window.
Search for "GitLens" and install it for enhanced Git capabilities.

- #### change default code editor
You can change the default code editor in your system to vscode. To do this, you can use the following command:
```cmd
  git config --global core.editor "code --wait"
```
#  Initialize folder into Git Repository.
- Create a folder and open in vs code.
- Open the terminal in VS Code.
- Initialize a new Git repository:
```cmd
  git init
```
- check status of the foldres an files.

```cmd
  git status 
```

## Commit


commit is a way to save your changes to your repository. It is a way to record your changes and make them permanent. You can think of a commit as a snapshot of your code at a particular point in time. When you commit your changes, you are telling git to save them in a permanent way. This way, you can always go back to that point in time and see what you changed.

## Steps of commit

![logo](https://app.eraser.io/workspace/SMlHs99FVb8wFX7uXTLP/preview?elements=PBx4CuCnDKSV09sU8nNxVw&type=embed)

1. write code

2. . Add your file
    ```cmd
      git add <FILE_NAME> <FILE_NAME> <FILE_NAME>
    ```
    - If you want to all the file :
    
    ```cmd
      git add .
    ```
3. commit
```cmd
  git commit -m "commit message"
  ```
  - Here we are committing the changes to the repository. We can see that the changes are now committed to the repository. The `-m` flag is used to add a message to the commit. This message is a short description of the changes that were made. You can use this message to remember what the changes were.

4. check status (optional)

```cmd
  git status
  ```
## Complete git flow A complete git flow

A complete git flow, along with pushing the code to github looks like this:
![View on Eraser](https://app.eraser.io/workspace/SMlHs99FVb8wFX7uXTLP/preview?elements=saaYh4YXnoXzKAPF2YJXgA&type=embed)
## Logs
The git log command is a powerful tool in Git that allows you to view the history of your repository. When used with the --oneline option, it presents this history in a simplified, condensed format. Here's a quick guide to help you understand and use these commands effectively.

#### What is git log?
git log displays the commit history of your repository. By default, it shows detailed information about each commit, including:

- Commit hash
- Author
- Date
- Commit message
#### Key Points About git log
- **Comprehensive History** : See all commits, from the most recent to the earliest.
- **Details** : Includes author, date, and the commit message for each commit.
- **Customizable** : Can be tailored with various options to show different levels of detail or specific information.

Example Usage :
```cmd
  git log
```
#### Simplifying with `--oneline`

Adding the `--oneline` option to git log condenses the output, showing each commit in a single line. This format includes:

- **Abbreviated Commit Hash** : Shorter version of the full commit hash.
- **Commit Message** : The first line of the commit message.

#### Key Points About `--oneline`
**Compact View** : Easier to scan through the commit history quickly.
** Abbreviated Hashes** : Shortened commit hashes for simplicity.
** Ideal for Summarizing** : Useful when you need a quick overview.

Example Usage :
```cmd
    git log --oneline
```
# .gitignore

The `.gitignore` file is a crucial component for managing Git repositories. It helps developers control which files and directories should be ignored by Git, preventing them from being tracked and versioned. This is particularly useful for keeping your repository clean and focused on the necessary files.

#### Key Points
- **Purpose** : `.gitignore` tells Git which files or directories to ignore, ensuring they are not committed to the repository.
- **Common Uses** : Ignoring build files, temporary files, configuration files, and dependencies that are not needed in the version control system.

### How to Create and Use a .gitignore File

#### Step-by-Step Guide
1. Create the .gitignore File
  -  In your project root directory, create a new file named `.gitignore`.

2. Add Patterns to .gitignore

- Each line in the `.gitignore` file represents a pattern for files/directories to ignore.

Example :
``` 
    # Ignore node_modules directory
    node_modules/

    # Ignore all .log files
    *.log

    # Ignore specific file
    secret.txt

```
# .gitkeep
When working with Git, you might encounter a file named .gitkeep. It’s not an official Git feature but a widely used convention. Here’s a quick guide to understanding and using `.gitkeep` effectively.

#### What is .gitkeep?
- **Purpose** : Keeps empty directories in Git repositories.
- **Function** : Ensures that directories without files are tracked by Git.
#### Why Use .gitkeep?
Git Basics: Git only tracks files, not empty directories. Without a file, empty directories won’t be committed.
Project Structure: Sometimes, you need to maintain a specific directory structure for your project. `.gitkeep`  helps achieve this by making sure the directories stay in the repo.

#### How to Use .gitkeep
1. Create an Empty Directory:

  - Navigate to your project directory.
  - Create the desired empty directory if it doesn’t exist.

2. Add .gitkeep:
- Inside the empty directory, create a file named .gitkeep.
![logo](https://app.eraser.io/workspace/SMlHs99FVb8wFX7uXTLP/preview?elements=s0eXJRwy1oRHmgIAnk_ZWg&type=embed)
#### Best Practices
- **Consistency** : Use .gitkeep consistently across your projects to avoid confusion.
- **Documentation** : Add a note in your project’s documentation explaining why and where you use .gitkeep.
- **Cleanliness** : Periodically check if the directories still need to be empty or if files have been added, making .gitkeep unnecessary.
