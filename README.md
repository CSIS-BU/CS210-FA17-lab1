# CS 210, Lab 1 -- When the remote repository is not originally empty (already has files/directory)

1. Install Git on your machine [Git](https://git-scm.com/)

1. Follow the provided link to create your own repository on GitHub

    * If you do not have a GitHub account, create one with your Bradley University e-mail address

1. First check the repository. If the repository is empty (has no existing files in it), then follow the instruction in [README-EmptyProject](README-EmptyProject.md); otherwise, continue the following instructions.

1. Since in this lab, you see the files README.md, README-EmptyProject.md, and .gitignore, you should continue with the following instructions.

    * Open a command prompt: since you have installed Git, you can run "Git CMD" (Windows' App) instead

    * If you are in Windows, your default directory would be C:\Users\[your login id]

    * Now, change directory to Desktop by the following command.

    **cd Desktop**

    * Enter the following command to get a copy of the remote repository on GitHub to your Desktop

    **git clone git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git**

    * Note: Here, you are set up to use SSH to connect to the repository. Thus, you'll have to follow the instructions provided in this URL [Help, I keep getting a 'Permission Denied (publickey)' error when I push!](https://gist.github.com/adamjohnson/5682757) and set up the SSH key for the access.

    * Note: Another way to do it is through HTTPS. That is, instead of adding the remote repository info through the command above, you can execute the following command:

    **git clone https://github.com/CSIS-BU/cs210-fa17-lab1-[YOUR ID].git**

    * Be careful about the step above. The [YOUR ID] part should match what you get under GitHub

    * Note: I'd like you to learn how to do both SSH and HTTPS. Due to time limitation, I'll let you work on the SSH part. If you still have difficulty working with SSH, you can use the HTTPS option instead.

1. Once you are done, there should be a **new sub-directory** created on your **Desktop** called "cs210-fa17-lab1-[YOUR ID]"

    * Now execute the following command.

    **cd cs210-fa17-lab1-[YOUR ID]**

    **echo "# CS 210, FA 17, Lab 1, [Your Name], [Your E-mail Address]" >> Lab1.txt**

    **git add Lab1.txt**

    **git commit -m "CS 210 Lab 1"**

1. The first time you commit with your changes, you'll be asked to set up your name and e-mail for the remote repository.

    * Read the instructions and you know you'll have to execute the following commands.

    **git config --global user.name "[Your User Name]"**

    **git config --global user.email "[Your e-mail address]"**

    * This only has to be executed once, which will be stored in the global setting.

1. Now upload the changes you made to the GitHub repository.

    **git push -u origin master**

1. Now login to your GitHub page and see if your repository does include the **Lab1.txt** file.

    * If so, you're now done with Lab 1. If not, please try again or contact the instructor for help.