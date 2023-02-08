My first readme
Resources Links
Resources to learn Git: https://docs.github.com/en/get-started/quickstart/set-up-git About READMEs: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes How to write a Git commit message: https://cbea.ms/git-commit/

Learning branching: https://learngitbranching.js.org/ Effective pull requests and other good practices for teams using GitHub: https://codeinthehole.com/tips/pull-requests-and-other-good-practices-for-teams-using-github/

Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

What is source code management What is Git What is GitHub What is the difference between Git and GitHub How to create a repository What is a README How to write good READMEs How to commit How to write helpful commit messages How to push code How to pull updates How to create a branch How to merge branches How to work as collaborators on a project Which files should and which files should not appear in your repo

Requirements
General A README.md file at the root of the alx-pre_course repo, containing a description of the repository A README.md file, at the root of the folder of this project (i.e. 0x01-git), describing what this project is about Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line. Your answer files should only contain the command, and nothing else

More Info
Basic usage At the end of this project you should be able to reproduce and understand these command lines:

$ git clone $ touch test $ git add test $ git commit -m "Initial commit" $ git push origin main

Tasks
Task 0. Create and setup your Git and GitHub account

Step 0 - Create an account on GitHub [if you do not have one already] You will need a GitHub account for all your projects at ALX. If you do not already have a github.com account, you can create an account for free (github.com)

Step 1 - Create a Personal Access Token on Github To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github. You can follow this tutorial to create a token (https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token). Step 2 - Update your profile on the Intranet Update your Intranet profile by adding your Github username. Step 3 - Create your first repository Using the graphic interface on the github website, create your first repository. Name: alx-pre_course Description: I'm now a ALX Student, this is my first repository as a full-stack engineer Public repo No README, .gitignore, or license Step 4 - Open the sandbox On the intranet, just under the task, click on the button and run to start the machine.

Once the container is started, click on to open a shell where you can start work from.

Step 5 - Clone your repository On the webterm of the sandbox, do the following: 1) git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-pre_course.git. Step 6 - Create the README.md and push the modifications Update your git identity: 1) git config --global user.email "you@example.com". 2) git config --global user.name "Your Name" Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin

Task 1. Repo-session: Create a new directory called 0x01-git in your alx-pre_course repo. Make sure you include a non empty README.md in your directory.

Task 2. Coding fury road: or the moment we have an empty project directory containing only a README.md. It’s time to code!

Inside 0x01-git:

Create these directories at the root of your project: bash, c, js Create these empty files: c/c_is_fun.c js/main.js js/index.js Create a file bash/alx with these two lines inside: #!/bin/bash and echo "ALX" Create a file bash/school with these two lines inside: #!/bin/bash and echo "School" Add all these new files to git Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

Task 3. Collaboration is the base of a company

branch is like a copy of your project. It’s used mainly for:

adding a feature in development collaborating on the same project with other developers not breaking your entire repository not upsetting your co-workers The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch update_script and in this branch:

Create an empty file named bash/98 Update bash/alx by replacing echo "ALX" with echo "ALX School" Update bash/school by replacing echo "School" with echo "The school is open!" Add and commit these changes (message: “My personal work”) Push this new branch Tips Perfect! You did an amazing update in your project and it’s isolated correctly from the main branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

Change branch to main Update the file bash/alx by replacing echo "ALX" with echo "ALX School is so cool!" Delete the directory js Commit your changes (message: “Hot fix”) and push to the origin Ouf, hot fix is done!

Task 4. Collaboration: be up to date

f course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – and only for this task – please update your file README.md in the main branch from GitHub.com. It’s the only time you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

Get all changes of the main branch locally (i.e. your README.md file will be updated) Create a new file up_to_date at the root of your directory and in it, write the git command line used Add up_to_date to git, commit (message: “How to be up to date in git”), and push to the origin

Task 5. HAAA what did you do???

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch update_script to main: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

HHHHHHHAAAAAAAA As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch update_script, and push the result to the origin.

At the end, you should have all your work from the branch update_script (new file and two updated files) and all latest main commits (new files, delete folder, etc.), without conflicts.

Task 6.Never push too much Create a .gitignore file and define a rule to never push ~ files (generated by Emacs). Tips (https://git-scm.com/docs/gitignore)
