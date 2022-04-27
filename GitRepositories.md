# ***Repositories; What is Git and how to use them.***

Very simply speaking, a repository is a set of files that you have assigned Git to pay attention to.
It keeps track of previous versions of the code that has been written. The benefits of maintaining copies of previous versions (aka Version Control) of the code is that if there are any errors or causes for corruption in the code. 

Version Control revisits previous versions of files and directories. From this you can revert to previous versions, track modifications to files and who made those changes, and you can also compare versions if a newer version has caused an issue.

There are three different types of Version Control Systems. They are:
- Local (LVCS) - One database accessible by one client
- Centralized (CVCS) - One database accessible by multiple clients
- Distributed (DVCS) - Multiple databses accessible by multiple clients.

Based on this knowledge, do you know which type of Version Control System Git is?.....<!--DVCS-->

If you're ready to start your coding journey you can follow a step by step process [here!](https://codefellows.github.io/setup-guide/) 

This entry will not get into any of the coding for sites (we'll get into that later). For now let's say you've created your first repository, written your code on your preferred text editing software, and are ready to publish your website. Publishing and editing your website can be done through many Text Editors, but it is important to know that this procedure can also be completed through your Ubuntu terminal.

## **ACP (Add, Control, Push)**

As I mentioned above it is important to know how to make updates to the repository from within your linux terminal.Remembering the commands from [Coder's Comp](CodersComp.md) you must navigate to the location of your local repository. From this location you can use the commands below: 

- `git status`
    - Any files in red are not the latest version and must be updated.
- `git add FILENAME(s)`
    - This command makes record which changes to be updated on the github repository.Multiple files may be added in one command just separate the names with a space. Also remember linux is Case sensative so pay attention to the FileName. (<-hint)
- `git commit -m "message"`
    - This step prepares the files above for the "push" command below which...
- `git push`
    - Takes a new snapshot of the repository and update from the local client as the current version of the code.
- `git pull`
    - Updates the local client with the version of code from the Github repository.

Click [Here](README.md) to return home