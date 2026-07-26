# DevOps Bootcamp for Beginners

![DevOps Illustration](image.png)

> Code is the dough and build is the bread.

## **Version Control**
----------------------------------------------
### Question
What is the difference between `git cherry-pick`, `git revert`, and `git reset`?

### Answer

#### 1. `git reset` — The Eraser
- Moves your current branch pointer backward.
- Removes commits from history in your local repository.
- Best used for fixing local mistakes before sharing your work.

**Analogy:** Ripping a few faulty pages completely out of your diary.

#### 2. `git revert` — The Safe Undo
- Creates a new commit that reverses the changes of a previous commit.
- Does not remove history.
- Best used for undoing an error on a shared public branch like `main` without rewriting history.

**Analogy:** Writing a new diary entry that says, "Ignore everything I wrote yesterday; it was a mistake."

#### 3. `git cherry-pick` — The Copy-Paste
- Applies a single commit from another branch onto your current branch.
- Keeps history intact and does not move branch pointers.
- Best used to bring a specific bug fix or feature from another branch without merging all of its changes.

**Analogy:** Seeing a great paragraph in someone else's book, photocopying it, and pasting it into your own book.

## **CICD Pipelines** 
----------------------------------------------

`YAML` - Yaml Aint Markup Language, here indentation is everything ! 

Core Actions/Keywords 

1. name  : used to define a workflow/job title. 
2. on    : defines triggers ( push, PR, schedule)
3. jobs  : to define jobs
4. steps : sequential commands or actions 
5. run   : shell commands to execute  
6. uses  : use prebuilt actions
7. with  : when we want to pass parameters in the actions 
8. env   : to set environment variable 
9. needs : to make one job dependent on another 