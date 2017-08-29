## Some Error Messages that you may encounter while doing the lab

1. If you encounter the following error message

    *error: src refspec master does not match any.*

    *error: failed to push some refs to 'git@github.com:CSIS-BU/cs210-fa17-lab1-[Your ID].git'*

    * This means that you did not "commit" the changes.

    * So after running the following command, the error should be gone.

    **git commit -m "CS 210 Lab 1"**

1. When you try to execute the "git push XXX" command, again, there may be another error message as follows.

    *Permission denied (publickey).*

    *fatal: Could not read from remote repository.*

    * This is because the initial instruction provided

    **git remote add origin git@github.com:CSIS-BU/cs210-fa17-lab1-[YOUR ID].git**

    requires you to set up your SSH key.

    * The instruction to do that is provided in this link [Help, I keep getting a 'Permission Denied (publickey)' error when I push](https://gist.github.com/adamjohnson/5682757)

    * Otherwise, you may execute the following command instead, and you will be prompted to enter your ID/Password on GitHub.

    **git remote add origin https://github.com/CSIS-BU/cs210-fa17-lab1-[YOUR ID].git**

1. More to come...