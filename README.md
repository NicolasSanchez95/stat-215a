# Repository for submitting labs for STAT 215A Fall 2024

## Setup

Your report and code will be submitted via GitHub. The following instructions will show you how to set up your GitHub account and configure a repository so that you can submit your assignments. This workflow is shamelessly copied (with slight modifications) from Chris Paciorek and Jarod Millman's STAT243 class in 2014.

1. Install Git on your system (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

1. Sign up for GitHub (https://github.com/).

1. Highly recommended: Go to https://education.github.com/students and sign up for the student pack. This will give you free access to GitHub Copilot. Do this sooner rather than later as the verification process can take a week.

Once you have completed these first steps, you are then ready to create your private GitHub repository for this class.

1. Locally on your machine, clone my stat-215-a repository: `git clone https://github.com/anthonyozerov/stat-215-a`. This will create a copy of the repository on your own computer.

1. On the GitHub website, log in and create a **private** remote repository called `stat-215-a`. Add me (*anthonyozerov*) as a collaborator for this repository (on https://github.com/USERNAME/stat-215-a, navigate to Settings -> Collaborators -> Add people).

1. Back in the terminal, set the origin of your local repository to be the remote repository that you just made. Change USERNAME in the command below to your username. This tells git which remote repository to push your changes to when you `git push`. First, enter the repository directory with `cd stat-215-a`, then point it to your private repo with `git remote set-url origin https://github.com/USERNAME/stat-215-a.git`. (Advanced: if you have SSH keys set up for github, you can use the SSH URL instead of the HTTPS URL).

1. Edit *info.txt* to reflect your own information.

```
name = "Jane Smith"
SID = "0123456789"
email = "jsmith@berkeley.edu"
github_name = "janesmith"
```

Now you're ready to push to your remote repository for the first time:

1. Check git status `git status`. You should see a bunch of text including `modified:   info.txt`.

1. Add the files (`git add info.txt`; feel free to also add the `.gitignore` with `git add .gitignore`) and commit (`git commit -m “Updated info.txt with my own information”`).

1. Push your changes to your copy of the remote repository (`git push` or sometimes `git push remote origin`)

1. Check that info.txt has been updated in your remote github repository by navigating to https://github.com/USERNAME/stat-215-a (change USERNAME to your username)

## Submitting your projects

To submit your projects, you will need to create a subfolder in your local `stat-215-a` folder called `lab1` (if you are submitting lab 1). The precise structure of the `lab1` folder is described in the `lab-instructions.pdf` file in the `stat-215-a-gsi` repo.

Note that GitHub cannot host files more than 100 MB. If you try to push a file larger than this, GitHub will cry. This means you should avoid pushing the data to your GitHub.  

When you are ready, you need to add, commit, and push the `lab1/` folder.

At the time when the lab is due, we will run a script that automatically pulls all of your assignments into my local versions of your `stat-215-a` repositories. Please make sure to submit your labs on time. `lab0` is a pretend assignment which you will complete to make sure that you are all clear on what to do.

Note: this document was originally written by Rebecca Barter in Fall 2017 and edited by successive GSIs to reflect the changes in the course.  
