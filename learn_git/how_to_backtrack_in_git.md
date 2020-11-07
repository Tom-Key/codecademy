### How to Backtrack

-  Git offers a few eraser-like features that allow us to undo mistakes during project creation. 

- `git show HEAD`
     - In Git, the commit you are currently on is known as the `HEAD` commit.

- `git chechout HEAD filename`: will restore the file in your working directory to look exactly as it did when you last made a commit.

---
- `git reset HEAD filename` *unstage* that file from the staging area
    - This command resets the file in the staging area to be the same as the HEAD commit.
    - It does not discard file changes from the working directory, it just removes them from the staging area.
    
- `git reset commit_SHA`
    - Creating a project is like hiking in a forest.
    - [如何使用git命令回滚到指定版本以及返回到新版本](https://www.jianshu.com/p/9ff4644b8790)
    
    