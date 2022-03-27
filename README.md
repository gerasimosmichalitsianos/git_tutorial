###### DESCRIPTION 

      This text-file follows a course from Udemy for using the Git command-line
      software. This is a good review of version control using the command-line
      with the git software.

###### SETUP 

      This tutorial is a Git command-line tutorial from Udemy. To get started, first we
      create a repository in Github using the web browser GUI interface. Then we open a 
      terminal and can run the following commands:

      First go to the appropriate directory:

      $ cd /home/gerasimos/Desktop/programming/GIT_TRAINING_UDEMY/projectone
      $ pwd
      /home/gerasimos/Desktop/programming/GIT_TRAINING_UDEMY/projectone

      Set up our repository in this local directory and link it to Github:
      $ git init
      $ touch README.md
      $ git add README.md
      $ git commit -m "first commit"
      $ git branch -M main
        
      Also set username and email:
      $ git config --global user.email "gerasimosmichalitsianos@gmail.com"
      $ git config --global user.name "Gerasimos Michalitsianos"
      $ git remote add origin https://github.com/gerasimosmichalitsianos/git_tutorial.git

      Push changes the remote repository (GitHub):
      $ git push -u origin main
      $ git push

###### ADDING FILES

      To add all files in a repository, use:
      $ git add .
 
      Or to add an individual file:
      $ git add <filename>

###### CHECKOUT OF REPOSITORY
   
     To download and check out an online remote repository, do:
     $ git clone username@host:/path/to/repository
     
     Or if over a local network, use:
     $ git clone /path/to/repository

     Example:
     $ git clone https://github.com/gerasimosmichalitsianos/git_tutorial.git

     This is how we can download a remote software project
     onto our local computer.

###### VIEWING HISTORY

     $ git log

###### UNDO

      If a mistake was made, but has not been pushed to remote repo.,
      then we can undo a commit with:
      $ git commit --amend

      Example:
      $ git commit -m "Initial commit"
      $ git add somefile.txt
      $ git commit --amend

###### VERSIONS

      Each commit (with push) may be thought of as a version of the project. 
      To this end, you can use this version number, which is a unique identifier.

      $ git reset --hard 43f634918c28c472acb7e6837907bda3620d6ca2
   
      Note that when running commands like these, files may be added or removed,
      depending on if files were added and/or removed with between commits. 
      The point is, changes are thrown away.

###### UPDATE LOCAL REPOSITORY TO MATCH SAME AS REMOTE

      To make the local repository match what is on the remote (e.g. Github),
      we can do:
      $ git push origin master
      
      or 
      $ git push origin master --force

###### BRANCHING

      Branches are used to develop isolated features. It should not interfere
      with the work of others. The master branch is the default branch. After
      work is done on a branch, the work can be merged onto the master branch.
      (once the new features are completed)

      Branches are like a copy of a whole project, but the edits/changes
      do not affect what other programmers are doing. The master branch
      is the default branch. You can mix branches together using a process
      called "merging"

      To create a branch:
      $ git checkout -b feature_z

      To go back to the master branch:
      $ git checkout master

      To delete a branch:
      $ git branch -d feature_z

      Remember, all this work is done locally. But if you don't delete
      branches, they will be put online (remote) when pushing to the repo.

      You can see which branches exist:
      $ git branch

      Several programmers might be working on the same project on
      different branches e.g.

      $ git checkout -b feature_y
      $ git checkout -b feature_z
      
      Now list the branches:
      $ git branch
      feature_y
      feature_x
      *master

      The "*" indicates which branch we are currently on.

      To switch to using a branch:
      $ git checkout feature_y

###### GIT SYNC AND MERGE

      If using an remote (online) repository, others can make
      changes at the same time. To turn the local project/repo.
      into the latest version, run:

      This will download the online changes and include them
      into the local project.

      $ git pull

      If you work in a branch, you can merge changes with: 
      $ git merge <branch_name>

      This can lead to possible conflicts.

###### GIT TAG

      Remember, we can see history with:
      $ git log

      To create a tag, we can do something like:
      $ git tag 1.0.0 43f634918c28c472acb7e6837907bda3620d6ca2

      This can be used to label major and/or minor versions in
      project.

###### LAST UPDATED

      Gerasimos "Geri" Michalitsianos
      gerasimosmichalitsianos@gmail.com
      27 March 2022
