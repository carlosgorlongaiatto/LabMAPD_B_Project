### How to set up a [Centralized Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows)

Accept the invitation (from GitHub or through the link) and clone the central repository:

`git clone https://<YourToken>@github.com/<YourUsername>/LabMAPD_B_Project`

* Note that this operation must be done only once.

Each time before starting the work session you must update your local main branch with respect to origin main (i.e. the remote branch on GitHub) to make sure you have everyone else's changes:

`cd ../LabMAPD_B_Project`

`git fetch origin`

`git merge origin/main`

After making some changes to one or more files you can see the state of your repository:

`git status`

Fisrt of all stage your file:

`git add <FileName>`

* Note that you can stage all the files you edited at once with:

  `git add .`

Then commit your files:

`git commit -m "SomeDescription"`

Finally you must push your changes up to the remote branch on GitHub:

`git push origin main`
