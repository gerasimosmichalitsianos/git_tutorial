###### DESCRIPTION 

      This text-file follows a course from Udemy for using the Git command-line
      software. This is a good review of version control. 


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

###### VIEWING DIFFERENCES BETWEEN COMMITS

     $ 

###### LAST UPDATED

      Gerasimos "Geri" Michalitsianos
      gerasimosmichalitsianos@gmail.com
      26 March 2022
