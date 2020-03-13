# Tool Time: Git, GitHub and GH Pages
## Installing Git
[Download and install Git](https://git-scm.com/downloads) if you haven't already. For Windows users, this will also install Git Bash, the command line terminal you'll be using to access Git features.

## Create GitHub Account
[Create a GitHub Account](https://github.com/) if you haven't already. Github is a company that has created a developer community around the Git technology but Git and GitHub are not the same. We'll be using GH to share our repositories and publish websites on [GH Pages](https://pages.github.com/).

## Command Line: Navigating the file system
Although there are GUI (Graphical User Interface) desktop applications available for using git, we recommend you start on the command line first. You can move to a GUI later once you understand the base functionality.

See:
- [Basics of BASH for Beginners](https://towardsdatascience.com/basics-of-bash-for-beginners-92e53a4c117a)
- [CLI (command line interface) Cheat Sheet](https://www.git-tower.com/blog/command-line-cheat-sheet/)

### The 3 commands you will use 80% of the time
- `pwd`: displays your 'present working directory'. This will usually default to your home folder when you first open your terminal.
- `ls`: lists the contents of your current directory. The `-l` flag lists extra information and `-a` lists hidden files. `-la` will list extra information and also all hidden files.
- `cd`: changes your directory based on the path you provide after the command (separated by a space). Examples:
  - `$ cd Documents/my-project`
  - `$ cd /path/to/my-project`
  - `$ cd ../..`: moves up two directories

Quality of life cli tips
- tab: auto-completes file names and directories
- up arrow: browse through command history

## URIs, URLs, and file paths
### Naming conventions
- Files should be named consistently
- File names should be short but descriptive (<25 characters)
- Avoid special characters or spaces in a file name
- Underscores or hyphens instead of spaces
- Use lower case characters when possible
- Default file name for html: index.html
- Default file name for css: styles.css or main.css
- Default file name for js: app.js or index.js
- Default file name for documentation README (located in the root directory of a project; extension can vary but is usually .txt. or .md)

## Activity: [Configuring Git](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
- Setting your name
- Setting your email
- Setting up your keys (optional)
  - [Why does GitHub recommend HTTPS over SSH?](https://stackoverflow.com/questions/11041729/why-does-github-recommend-https-over-ssh)
  - [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Top Git commands
- `$ git status`: Show the working tree status. This gives you the big picture status of your project.
- `$ git add`: Add file contents to be committed (also called the staging area). You need to explictly tell Git what changes you want to commit to your repository. It seems unneccessary at first but there's a good reason for this.
- `$ git commit`: Record changes to the repository. This "saves" the changes that were added earlier to your repo. You will usually include the `-m` flag to add a comment (which is mandatory).
- `$ git push`: "Push" your local changes to a remote repo (usually a GitHub repo).
- `$ git pull`: "Pull" changes from a remote repo to your local repo.

## Cloning a repo from GitHub
### Option 1: Upload files and clone
1. Create empty GH repo with initialized README.md
2. Drag and drop files into your repo
3. Copy the clone url (look for the big green button on the main repo page that says "Clone or download")
3. Clone repo to your file system with `git clone [url you just copied]`

### Option 2: Push from existing local repo
1. Create empty GH repo WITHOUT initialized README.md
2. Follow listed instructions for "*…or push an existing repository from the command line*"  

**Important: Do not create a repo inside another repo**

### Activity: Publish a website using GH Pages
Follow the instructions in this article to publish a website to your main GH Pages account:

[The Beginners Guide to Github Pages](https://www.ostraining.com/blog/coding/github-pages/)
