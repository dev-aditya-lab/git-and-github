
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

![logo](https://app.eraser.io/workspace/SMlHs99FVb8wFX7uXTLP/preview?elements=PBx4CuCnDKSV09sU8nNxVw&type=embed)

- write code, then

- . Add you file
    ```cmd
      git add <FILE_NAME> <FILE_NAME> <FILE_NAME>
    ```
    - If you want to all the file :
    
    ```cmd
      git add .
    ```
## Support

For support, email fake@fake.com or join our Slack channel.


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`API_KEY`

`ANOTHER_API_KEY`


## Features

- Light/dark mode toggle
- Live previews
- Fullscreen mode
- Cross platform


![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)


## Demo

Insert gif or link to demo


## Usage/Examples

```javascript
import Component from 'my-project'

function App() {
  return <Component />
}
```


## Related

Here are some related projects

[Awesome README](https://github.com/matiassingers/awesome-readme)

