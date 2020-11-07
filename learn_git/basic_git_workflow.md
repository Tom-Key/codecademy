### Basic Git Workflow


![](https://content.codecademy.com/courses/learn-git/revised-git-diagram/git%20workflow_fullwidth.svg)
- `git init`: *initialize* sets up all the tools Git needs to begin tracking changes made to the project
- `git status`: check the status of those changes of the working directory
- `git add [filename]`:The file needs to be added to the staging area in order for Git to start tracking.
- `git diff [filename]`:check the differences between the working directory and the staging area
- `git commit -m "Complete first line of dialogue"` : permanently stores changes from the staging area inside the repository.
    - Must be in quotation marks
    - Written in the present tense
    - Should be brief (50 characters or less) when using `-m`
- `git log`:view commits stored chronologically in the repository