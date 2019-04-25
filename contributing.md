Guidelines - 9by10
===================

## Reporting
### Guidelines for Reporting Issues 
Before creating or placing any new issue, please go through the following guidelines :
1. Before placing a bug or new feature, make sure that you have the latest version of website running & all the cache is removed.
2. Also make sure to check whether the Issue has already been reported before in advance.
3. Make sure to follow the Issue Tracker template for Bug or Feature request & Fill all the necessary fields required, applicable for your required.
4. Try to include url, screenshot & detailed explaination about the Bug in the Issue Tracker for easy & quick resolution.

## Coding
### Contributing Guidelines
1. Before starting work on any Issue, make sure that the Issue in not assigned for any other person & the Issue must be assigned to you only.
2. Always pull the latest code from the master branch before starting the work.
3. If you are unable to understand the issue or unable to reproduce it, try consulting the person who raised the Issue & get to understand the full details about the Issue.
4. Never push non-working code to Git.
5. Always branch-off of master while working on any new Issue or feature.
6. Always keep your local master in sync with remote master using git pull --rebase (rebasing always for a cleaner way of merging without unnecessary commits when merging http://stackoverflow.com/a/2472600/4058128 )
7. Follow the below Git workflow for working on any Issue.
8. Do not start working on any other Issue without finishing the present one.

### Git Workflow 
1. git pull : For getting all latest code from Git.
2. git branch -b M-#123 - To make a new branch with the Issue number (Ex: #123)
3. git add : After making all required changes, use this command to add the changed files for commiting.
4. git commit : Type this command & press enter to write the commit message. Check below for Commit Message Guidelines.
5. git push origin M-#123 : Push your code to Git using this Command. Here M-#123 is the branch name.
6. Now raise a Pull Request with the below given guidelines for passing it to review stage  .
7. After the review, if there are any changes suggested, use this commands to work on them.
8. git checkout master
9. git pull
10. git checkout M-#123
11. git rebase master : Resolve any rebase conflicts  & then use this command (https://stackoverflow.com/a/11710051) : git rebase --continue
12. Now make all necessary changes as suggested by the reviewer & then follow below commands.
13. git add
14. git commit --amend
15. git push origin M-#123
16. Repeat the same till the PR is accepted & Merged.

### Git Commit Message Guidelines
1. Always use the Issue Number & Issue Name in the commit message followed by the short note about the changes made.
    Ex : #123 - Issue Title.<br>
    Removed the styling of adding extra padding from custom.css
2. Use the present tense ("Add feature" not "Added feature")
3. Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
4. Limit the first line to 72 characters or less
5. Reference issues url after the first line.
6. After all these, add a line in the following manner : 'Fixes Sunil02324/9by10-Tracker#123' : where #123 is the issue number.

### Pull Request Guidelines
1. Title of the Pull request must be Issue number followed by the name. Ex :  #123 - Issue Name
2. In the description, Include all the details about the changes made by you and how to test the changes. Include screenshot if the issue is related to some styling.
3. Add the reviewers accordingly for the required Issue.
4. Notify the Reviewers to Get it accepted & merged to the main branch.
5. If any changes are suggested, make necessary changes & followup with the reviewers accordingly.
