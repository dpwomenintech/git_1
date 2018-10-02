## GitHub Basics!
## Note on copy and paste using Git Bash
When you have copied something and would like to paste it into the Git Bash terminal, the traditional Ctr+V will not work instead you need to use Shift+Insert to paste from the clipboard.

### Clone this repository using
```
git clone https://github.com/dpwomenintech/git_1.git
```

### Navigate to the repository 
Use the command ```cd git_1``` (change directory command depending on what the folder name is).

If you run the command ```ls``` it will list out all of the files currently in the directory.

### Creating a Branch
This branch is where you will be making your changes

```
git checkout -b YOURNAME
```
This command will make a new branch called YOURNAME

When you create a new branch you are creating a copy of the repository where you can safely experiment without affecting the original copy.

### Working on your branch
Ensure that you are on your newly created branch by running ```git branch``` this should list all of your branches and there will be an * next to the branch you are currently working on.

You now need to navigate into the ContactsList directory and create a new text file named FirstNameLastName.txt, where you will list your name, phone number, best email to reach you and your favorite food. This will serve as a contacts list where later in the year you are able to contact fellow team members.

Edit the text file by opening the text file in any text editor ie. Notepad, Notepad++, Vim.

In the future you may have multiple branches you are working on. To switch between these branches use the checkout command ```git checkout BRANCHNAME```

#### Creating a text file
You can create a text file many different ways one way is to use git bash by running ```touch fileName.txt``` or by right clicking in the directory in file explorer and selecting "New" then "Text File"

### Commit your code
Commiting your code is essentially taking a snapshot of the work you have done since the last snapshot. You should commit your code every time there is a significant change or you are done working for the period/day.

To see your new changes run the command ```git status``` which will tell you which files have changed. 

You then need to stage these files to be apart of your commit. We do this by running ```git add .``` (this will add all changed files) or if you want a specific file added ```git add filename```

If you now run ```git status``` it will show all of the files you staged in green and the ones that aren't staged in red.

Lastly you need to add a commit message to your staged files to summarize the changes do this by running ```git commit -m "commit message goes here"```

Having clear and concise commit messages is extremely important. When you need to revert to a previous version clear commit messages will make your life easier. Remember for potential job/internship opportunities you may want to show off work in Github so clear and concise commit messages will also help you in this situation.

After commiting your code you are now able to push your changes to Github.

### Pushing your changes
When you are finished working, or it is the end of the period you need to push your work to Github so you have a safe backup.

Run the command from your working branch ```git push --set-upstream origin branchName``` this tells git that this is your upstream for your branch. This only needs to be run when it is your first commit on the branch.

After running this command once, you should be able to just run ```git push``` to push to your branch on Github.

### Pull Request
When you have completed all of the necessary tasks, and successfully pushed to your branch on Github you are going to need to open a pull request for an administrator to view your changes and incorporate into the master (protected branch).

Pull requests are useful as they group all of your branch changes together to be reviewed and incorported into the master branch.

To open a pull request follow this [guide.](https://services.github.com/on-demand/github-cli/open-pull-request-github)

[Guide created by Dos Pueblos Engineering Academy]
