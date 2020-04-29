# Git(hub) webinar OSCR – 29-04-2020
Ana Martinovici (assistant professor of marketing  attention, decision making, Bayesian statistics)
Github.com/anamartinovici/githubfun

## News
•	R-Ladies Netherlands book club: rladiesnl.github.io/book_club
•	How to use R and the tidyverse to clean, plot and analyze data: github.com/aschetti/ERIM2020_intro_tidyverse

## Why we should use version control
Best practice: use version control from the start of the project and document your code. It will be shareable more easily.

Why version control? Some research goals: 
- Collaborate with co-authors: you can work on the same project (repository) with more people
- Contribute to ongoing projects: this is possible even when you are not an official collaborator on the github repository
- Share your work with the world: you can make your repos public or private and also add a (software) license to the repository
- Reproducible results: if you can take the original data and original computer code used to analyze the data and reproduce all of the numerical findings from the study. Spectrum:

[spectrum]()

Goal: reproduce all results and nothing but the results included in the current version of the paper and previous analyses as fast and easy as possible. 
- Best case scenario: raw data > cleaning/processing > processed data > analysis > results
- Most likely scenario: raw data v4 > cleaning/processing > processed data v10 > analysis > results v50

Things that can go wrong without version control:
- Laptop/external HD explodes
- Overwriting files, but also not overwriting files
- Forgetting which of the final files is really final
- Change file X, but forget to update all the other files/results that depend on it
- Software changes

Version control:
•	Time travel
•	Safe place for your data and code
•	Notes to your future self

Git: formal version control system. Developed by Linus Torvalds (used to manage the course code for Linux). Tracks content: source code, data analysis projects, websites, presentations, manuscripts.
Github: home for git repositories, interface for exploring public git repositories. A safe place to keep code and data. Additional benefits: issues (notes to yourself or collaborators), projects, wiki, insights.

Why use GitHub?
- Facilitates exploring code, tracking issues, learning from others
- Lowers the barriers to collaboration:
 - Email: “there’s a type in your code in file X line X” VS
 - Pull request: “here’s a correction to your code”
- Free for researchers and students

## How to use version control
General idea
[image_general_idea]()

Vocabulary
- Repository (repo): folder containing all tracked files as well as the version control history
- Commit: snapshot of changes made to the staged file(s), to save a snapshot of changes made to the staged file(s)
- Stage: staging area holds the files to be included  in the next commit; to mark a file to be included in the next commit
- Track: a tracked file is one that is recognized by the git repository
- Branch: a parallel version of the files in a repository
- Local: version of your repo on your pc
- Remote: version of your repo stored on a remote server, e.g. Github
- Clone: local copy of a remote repo on your PC
- Fork: copy of another user’s repo on GitHub, to copy a repo to your own account. Changes made to the original repo are not changed in your forked repo (unless you pull the changes of that repo again)

See slides...

Link: [Setting up Git with RStudio](http://www.geo.uzh.ch/microsite/reproducible_research/post/rr-rstudio-git/)
In RStudio: Tools > Global options > Git/SVN: make sure that Enable version control interface is checked, that R knows where to find git.

Create your first repo: online and offline
- Internet: Go to your github account > Create a new repository
 - Give it a name (no spaces)
 - Always initialize with a readme
 - This creates an online version, to make changes, you need to clone the repo to your PC
-	Local:
 - On github, click Clone or download and copy the hyperlink
 - In RStudio, go to New project  Version control  Git  paste repository URL and choose a location to save the local copy
 - In the RStudio project, there should be a Git tab (topright panel).

Working in a local repo
-	Create files like you are used to in the folder on your local PC. Using R is not necessary, but you can just use RStudio to make commits and push changes
-	Files that are changed or newly created will appear in RStudio in the Git tab
-	In this Git tab, click the file/change that you wish to save: you will now commit the changes (“create a shipping label”)
 - Commit > in the review changes window, write a short commit message (what did you change exactly/why?) > In present tense 😊 
 - Click Commit
 - Click Push
 - After pushing, the changes are also visible in your online version on GitHub
