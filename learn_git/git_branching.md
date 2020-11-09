### Git Branching

![](https://content.codecademy.com/courses/learn-git/git-diagram-1.svg)
- `git branch`:use the command below to answer the question: “which branch am I on?”
    -  the `*` (asterisk) is showing you what branch you’re on
    - New Branch is a different version of the Git project. It contains commits from Master but also has commits that Master does not have.
    - Branch name cannot contain whitespace
    
- `git branch [new_branch]` create a new branch
- `git checkout branch_name`switched to a branch
- `git merge`:include all the changes made to the fencing branch on the master branch

- `merge conflict`
    ``` 
    CONFLICT (content): Merge conflict in [filename]
    Automatic merge failed; fix conflicts and then commit the result.

    <<<<<<< HEAD
    master version of line
    =======
    branching version of line
    >>>>>>> fencing
    ```
- `git branch -d branch_name`:delete the specified branch from your Git project 