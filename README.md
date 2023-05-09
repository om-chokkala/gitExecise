# gitExecise

Creating a git remote repository from a local repo. I have followed the below commands.

    git remote add origin <url>
    git push -u origin

Local repo and gitHub have different histories. There is a problem when merging master(local git) branch to the Github repo main (default) branch.
I have used the below commands to solve the problem 

   git checkout master
   git branch main master -f    ---> used it to make both histories equal  
   git checkout main   
   git push origin main -f
    
