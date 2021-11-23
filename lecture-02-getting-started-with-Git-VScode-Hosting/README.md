 # **Getting started with Git, VSCode and Hosting**

 <p>&nbsp;</p>

# WHAT IS GIT?

- Git is a free and open-source distributed **version control** system designed to handle everything from small to very large projects with speed and efficiency.

- It is a record-keeping mechanism. If any changes are done then one gets to know who did it and what were the changes.
- It is a client/local storage
<br/><br/>
><h3>What is version control in git?</h3>

- Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

<p>&nbsp;</p>

# HOW DOES GIT WORK?

With Git, a developer can have a full history of their code repository locally. 

Traditionally, a Git workflow will involve the following steps:
1. Creating a repository 
2. Adding files to your repository
3. Making changes in the files
4. Saving those changes with good commit messages so that the history of the entire code can be tracked.
5. Pushing your changes to the main branch
<br/><br/>
><h3>Why do we have to push the changes?</h3>

- All the changes that you did until now were being saved locally. But your computer might crash and you might lose all these changes. We push the changes so that the code will be available on the cloud and we can share and collaborate with others. 

<p>&nbsp;</p>

# WHAT IS GITHUB?
- GitHub is a web-based interface that uses Git, the open-source version control software that lets multiple people make separate changes to web pages at the same time.
<br/><br/>

><h3>Difference between Git and GitHub:</h3>
* Git is a local change tracking mechanism whereas GitHub is a cloud storage & allows collaboration.
<br/><br/>
><h3>Why GitHub?</h3>
- allows real-time collaboration
- it encourages teams to work together to build and edit their site content
<p>&nbsp;</p>

# HOW DOES GITHUB WORK?

If you don't need to work with files locally, GitHub lets you complete many Git-related actions directly in the browser, including :

><h3>Creating a repository</h3>
- You can store a variety of projects in GitHub repositories. While creating a new repository add a name without any space and a 
small description of what is present in the repository. 
- Whenever a new repository is created, a .gitattributes file is automatically generated. It is a hidden file used by the Github desktop to do checks.

><h3>Cloning a repository </h3>
- When you want to make changes to a repository, you can clone it and work in that repository on your local machine 
><h3>Forking a repository</h3>
- you can fork a repository to create a copy of the repository and make changes without 
affecting the original repository. 

><h3> Being social</h3>
- You can interact with people, repositories, and organizations on GitHub. See what others are working on and who they're connecting with from your dashboard.

<p>&nbsp;</p>

# KNOWING HOW A DEV IN A TEAM WORKS?


When working in a team, you can work in different branches.
><h3>Branching </h3>
- Use a branch to isolate development work without affecting other branches in the repository. Each repository has one default branch and can have multiple other branches</h3>
><h3>Pull requests</h3>
- Let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base(main) branch. If you're working in the shared repository model, it is advisable to use a separate branch for your pull request.
><h3>Pull origin </h3>
- When you want to make changes in the repository, always remember to pull origin to have all the changes on your local machine. Changes are pulled from server to client.
><h3>Push origin</h3>
- When you are done making changes locally u need to push them so that everyone in the team can view your work. Changes are pushed from client to server.
<p>&nbsp;</p>

# ALL ABOUT COMMITS!

><h3>What is commit?</h3>
- change and save (in simple terms)
- In Git, a commit is a snapshot of your repository at a specific point in time.
<br></br>
><h3>Types of Commit:</h3>
1. feat: The new feature you're adding to a particular application
2. fix: A bug fix
3. style: Feature and updates related to **styling**
4. refactor: Refactoring a specific section of the codebase
5. test: Everything related to testing
6. docs: Everything related to documentation
7. chore: Regular code maintenance.
<br></br>
><h3>What is a good commit message?</h3> 
- Specify the type of commit
- Separate the subject from the body with a blank line
- Your commit message should not contain any whitespace errors
- Remove unnecessary punctuation marks
- Do not end the subject line with a period
- Capitalize the subject line and each paragraph
- Use the imperative mood in the subject line
- Use the body to explain what changes you have made and why you made them.
- Do not assume the reviewer understands what the original problem was, ensure you add it.
- Do not think your code is self-explanatory
- Follow the commit convention defined by your team
<br></br>
><h3>Reverting a commit</h3>
- The git revert command is used for undoing changes to a repository's commit history.
_(just like undo)_
<p>&nbsp;</p>

# HOW DOES THE INTERNET WORK?
><h3>Example </h3>

- When you type the name of a website, the browser goes and asks the server if it has this website. 
- There are 2 types of servers involved here: <br>
server 1 - knows where the website is/tells address of the website<br>
server 2 - the one who hosts the website.<br>
server 2 then gives the information to server 1 which further gives it to the browser and then the browser downloads it for you.
<p>&nbsp;</p>

# WHAT IS HOSTING?
Web hosting is an online service that allows you to publish your website on the internet.
Anyone who has access to the internet has access to your website

_Not hosting a good app is like baking a cake, decorating it, but not eating_ :(
  <p>&nbsp;</p>

# HOW TO HOST YOUR WEBSITE FOR FREE?
_Now, let's enjoy the cake!!!!_

There are many platforms to host your website for free like Vercel, Netlify, GitHub Pages, Heroku, etc.


Netlify has GitHub integration and is very simple to use.

><h3>How to use netlify?</h3>
- sign up to netlify using your GitHub login
- Select a new site from a repository
- Select your GitHub repository
- And your website will get deployed
- you can even edit the domain name
<br></br>
><h3>What is continuous deployment?</h3>
- Every time you change something on the website and push it on GitHub it will be published automatically
on netlify.
<br></br>

_Some things to remember:_
- main file should be index.html otherwise netlify won't deploy
- netlify deploys only from the main branch

<p>&nbsp;</p>

# GETTING FAMILIAR WITH VSCODE  
An IDE (integrated development environment) made by Microsoft for Windows, Linux, and macOS.
>Makes life easier with its ample amount of extensions

  A few examples:<br>
  - Live Server -  Launch a development local Server with live reload feature for static & dynamic pages.<br>
  <a href="https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer">Know more</a>
  - Prettier - Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.<br> <a href="https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode">Know more</a>
<br></br>
><h3>Integration of github (connects with github):<h3>
* Add a GitHub account to sign in to Visual Studio Code.
* Initialize a Git repository and push it to GitHub by using Visual Studio Code
* Make and push commits to your remote branch using Visual Studio Code

 _Right from creating a repo to pushing it, all can be done in this space!!!!_
<br></br>
><h3>Some shortcuts to save time</h3>

- Show and hide terminal: ctrl + `
- Show and hide sidebar: ctrl + b 
- Open any file: ctrl + p
- Access all available commands based on your current context : ctrl+shift + p
- Jump to symbols: ctrl + p and then type '@symbol'
- Jump to line : ctrl + p and then type ' : line-number '
- Toggle wrap: alt+z
- Code formatting: alt + shift + f

<p>&nbsp;</p>

***Know more about how to open PR's in a repo which you don't own*** 👇<br>
https://youtu.be/jUxy4WNdc0s


