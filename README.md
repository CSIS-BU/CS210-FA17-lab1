# CS 210, Lab 1

1. Install Git on your machine [Git](https://git-scm.com/)

1. Follow the provided link to create your own repository on GitHub

    1.1 If you do not have a GitHub account, create one with your Bradley University e-mail address

1. First check the repository. If the repository is empty (has no existing files in it), then follow the instruction in [README-EmptyProject](README-EmptyProject.md); otherwise, continue the following instructions.

1. Since in this lab, you see the files README.md, README-EmptyProject.md, and .gitignore, you should continue with the following instructions.

    Enter the following commands under command prompt.

    git clone git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git

    Note: Here, you are set up to use SSH to connect to the repository. Thus, you'll have to follow the instructions provided in this URL [Help, I keep getting a 'Permission Denied (publickey)' error when I push!](https://gist.github.com/adamjohnson/5682757) and set up the SSH key for the access.

    Note: Another way to do it is through HTTPS. That is, instead of adding the remote repository info through the command above, you can execute the following command:

    git clone https://github.com/CSIS-BU/cs210-fa17-lab1-[YOUR ID].git

    Be careful about the step above. The [YOUR ID] part should match what you get under GitHub

1. Once you are done, there should be a new sub-directory created under the current directory called "cs210-fa17-lab1-[YOUR ID]"

    Now execute the following command.

    cd cs210-fa17-lab1-[YOUR ID]

    echo "# CS 210, FA 17, Lab 1, [Your Name], [Your E-mail Address]" >> Lab1.txt

    git add Lab1.txt

    git commit -m "CS 210 Lab 1"

    git push -u origin master

1. Once you are done, login to your GitHub page and see if your repository does include the Lab1.txt file.

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

## Other related notes

1. From time to time, the instructor may update the instructions on the labs to clarify a few things. Once you have created your own repository from the link provided, you won't get those chnages automatically.

1. To get the updates, you have to execute the following command (through Git bash and command prompt/terminal)

    * First, go to the corresponding folder where you keep the repository.

    * Then, do the following command (assume that your current branch is "master" and the original repository is located at "CSIS-BU/cs210-fa17-lab1.git")

    git branch master

    git pull https://github.com/CSIS-BU/cs210-fa17-lab1.git master

    git push origin master

1. After these steps, both your local and remote repositories will get the latest update.

* Note: You may be asked to fix some conflicts (if you changed some files), which you should not have to worry in this lab.

* Reference: [Merging an upstream repository into your fork](https://help.github.com/articles/merging-an-upstream-repository-into-your-fork/)
