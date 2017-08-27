# CS 210, Lab 1

1. Install Git on your machine [Git](https://git-scm.com/)

1. Follow the provided link to create your own repository on GitHub

   1.1 If you do not have a GitHub account, create one with your Bradley University e-mail address

1. In your repository, your will see an initial page with instructions (all command prompts).

   You now enter the following commands under command prompt.

   echo "# CS 210, FA 17, Lab 1, [Your Name], [Your E-mail Address]" >> Lab1.txt

   git init

   git add Lab1.txt

   git commit -m "CS 210 Lab 1"

   git remote add origin git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git
   
   Note: Here, you are set up to use SSH to connect to the repository. Thus, you'll have to follow the instructions provided in this URL [Help, I keep getting a 'Permission Denied (publickey)' error when I push!](https://gist.github.com/adamjohnson/5682757) and set up the SSH key for the access.
   
   Note: Another way to do it is through HTTPS. That is, instead of adding the remote repository info through the command above, you can execute the following command:
   
   git remote add origin https://github.com/CSIS-BU/cs210-fa17-lab1-[YOUR ID].git

   Be careful about the step above. The [YOUR ID] part should match what you get under GitHub

   git push -u origin master

1. Under the condition that you would like to push an existing repository to the GitHub

   You can do

   git remote add origin git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git

   git push -u origin master

1. Once you are done, login to your GitHub page and see if your repository does include the README.md file.

   If not, please try again or contact the instructor for help.
   
## Some Error Messages that you may encounter while doing the lab

1. If you encounter the following error message

   error: src refspec master does not match any.
   
   error: failed to push some refs to 'git@github.com:CSIS-BU/cs210-fa17-lab1-[Your ID].git'
   
   This means that you did not "commit" the changes.
   
   So after running the following command, the error should be gone.
   
   git commit -m "CS 210 Lab 1"

1. When you try to execute the "git push XXX" command, again, there may be another error message as follows.

   Permission denied (publickey).
   
   fatal: Could not read from remote repository.
   
   This is because the initial instruction provided
   
   git remote add origin git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git
   
   requires you to set up your SSH key.
   
   The instruction to do that is provided in this link [Help, I keep getting a 'Permission Denied (publickey)' error when I push](https://gist.github.com/adamjohnson/5682757)
   
   Otherwise, you may execute the following command instead, and you will be prompted to enter your ID/Password on GitHub.
   
   git remote add origin https://github.com/CSIS-BU/cs210-fa17-lab1-[YOUR ID].git
   
1. More to come...
