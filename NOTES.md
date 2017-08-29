## Other related notes

1. From time to time, the instructor may update the instructions on the labs to clarify a few things. Once you have created your own repository from the link provided, you won't get those changes automatically.

1. To get the updates, you have to execute the following command (through Git bash and command prompt/terminal)

    * First, go to the corresponding folder where you keep the repository.

    * Then, do the following command (assume that your current branch is "master" and the original repository is located at "CSIS-BU/cs210-fa17-lab1.git")

    **git branch master**

    **git pull https://github.com/CSIS-BU/cs210-fa17-lab1.git master**

    **git push origin master**

    * Note: the address in the second command above will/should be provided; otherwise, you won't be able to access the original lab files with the instructor's updates.

1. After these steps, both your local and remote repositories will get the latest update.

* Note: You may be asked to fix some conflicts (if you changed some files), which you should not have to worry in this lab.

* Reference: [Merging an upstream repository into your fork](https://help.github.com/articles/merging-an-upstream-repository-into-your-fork/)

1. If you want to change the associated remote repository, you can do the following.

    * Check the current remote repo setting

    **git remote -v**

    * Once you see the remote setting, such as

    *origin  git@github.com:CSIS-BU/CS210-FA17-lab1.git (fetch)*
    
    *origin  git@github.com:CSIS-BU/CS210-FA17-lab1.git (push)*

    * You may remove them by doing

    **git remote remove origin**

    * And you can add the same remote repo through HTTPS with the following command.

    **git remote add origin https://github.com/CSIS-BU/CS210-FA17-lab1.git**

    * Check again on the remote repo setting.

    **git remote -v**