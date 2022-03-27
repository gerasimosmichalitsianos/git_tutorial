###### Description

      This text-file follows a course from Udemy for using the Git command-line
      software. This is a good review of version control. 


###### Setup

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
        
      $ git remote add origin https://github.com/gerasimosmichalitsianos/git_tutorial.git
      $ git push -u origin main
      $ git push

