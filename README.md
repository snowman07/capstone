# capstone

Repo for capstone testing

# Deployment using Bash with NPM

> I used Bash with NPM. Just go to the project directory using BASH

Run this command:

- export GIT_USER="snowman07"
- npm run deploy

<br/><br/><br/><br/>

# Golden Rule

- Always `git pull` when starting to code and when creating a branch to get the most updated code.
- Always `git push` when done coding.
- Always `create a "branch"` when doing your task to avoid merge conflict. Work on your code using that branch. <br/><br/>

# Commands to create a branch

> Follow git commands in order

| <center>COMMANDS</center>                      | <center>COMMENT/S</center>                                                                                                                                                                               |
| :--------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| git branch                                     | <ul><li>Make sure you're in `development` branch</li><li>Notice the asterisk \*</li></ul>                                                                                                                |
| git pull                                       | <ul><li>Golden rule: always git pull</li><li>To make sure you get the most updated code</li></ul>                                                                                                        |
| git branch `newBranch`                         | <ul><li>To create a new branch</li><li>Change `newBranch` into your desired branch name</li><li>Branch name must `include your name` for identification</li></ul>                                        |
| git checkout `newBranch`                       | <ul><li>To go to the new branch created</li><li>`newBranch` is your branch name</li></ul>                                                                                                                |
| git push -u origin `newBranch`                 | <ul><li>Not necessary but highly suggest to do it in order to track the history of this branch remotely(cloud/gitlab)</li><li>To check, go to gitlab repo/project, `newBranch` should be there</li></ul> |
| git branch                                     | <ul><li>Not necessary but it's always good to double check the branch you're in.</li><li>This time, you should be in `newBranch`</li></ul>                                                               |
| `CODE TIL YOU DROP AND DONT FORGET TO SAVE!!!` |                                                                                                                                                                                                          |
| git add .                                      | <ul><li>To add the code</li></ul>                                                                                                                                                                        |
| git commit -m "descrition here"                | <ul><li>To save the code locally (in your machine)</li><li>Include ""</li></ul>                                                                                                                          |
| git push                                       | <ul><li>Command to push the code in cloud/gitlab specifically located in `newBranch` you created</li></ul>                                                                                               |
| git diff `mainBranch` `newBranch`              | <ul><li>Not necessary but it's the command to check the differences made from newBranch to mainBranch</li><li>mainBranch in this project is the `development branch`</li></ul>                           |

> If everyone agrees that the code in `newBranch` is worthy to add in mainBranch (`development`), it's time to `merge the code`.

<br/><br/>

# Commands to merge

> Follow git commands in order

| <center>COMMANDS</center>  | <center>COMMENT/S</center>                                                                                                              |
| :------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------- |
| git branch                 | <ul><li>Not necessary but to make sure which branch you're in</li></ul>                                                                 |
| git checkout `development` | <ul><li>To merge, `make sure that you're in the main branch` (in this project, it's the `developmnet branch`)</li></ul>                 |
| git pull                   | <ul><li>Golden rule: always git pull</li></ul>                                                                                          |
| git merge `newBranch`      | <ul><li>Command to merge the code from `newBranch` to main branch (`development branch`)</li></ul>                                      |
| git push                   | <ul><li>At this point, merge is successful.</li><li>Code from `newBranch` is now merged to main branch (`development branch`)</li></ul> |

> If the team decides to delete newBranch, follow below command

<br/><br/>

# Commands to delete branch

> Follow git commands in order

| <center>COMMANDS</center>            | <center>COMMENT/S</center>                                                                                                           |
| :----------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| git checkout `development`           | <ul><li>To delete a branch, make sure you're in main branch (`development`)</li></ul>                                                |
| git branch                           | <ul><li>Not necessary but to make sure that you're in `development branch`</li></ul>                                                 |
| git branch -d `newBranch`            | <ul><li>Command to delete the branch `locally (in your machine)` </li></ul>                                                          |
| git branch                           | <ul><li>`newBranch` should disappear in your editor</li></ul>                                                                        |
| git push origin --delete `newBranch` | <ul><li>To delete the branch `remotelly (in cloud/gitlab)`</li><li>Check gitlab repo/project, `newBranch` should disappear</li></ul> |

<br/><br/>

# Helpful Links

- [Docusaurus documentation](https://docusaurus.io/)
- [Git Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=The%20overall%20flow%20of%20Gitflow,branch%20is%20created%20from%20main&text=When%20a%20feature%20is%20complete%20it%20is%20merged%20into%20the,branch%20is%20created%20from%20main)
- [Youtube git branching and merging tutorial](https://www.youtube.com/watch?v=hufGg2mf7eA)
