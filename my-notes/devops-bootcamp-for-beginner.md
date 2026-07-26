# DevOps Bootcamp for Beginners

![DevOps Illustration](image.png)

**DevOps --> DEV + OPS**

> Code is the dough and build is the bread.

## Version Control
=======
----------------------------------------------
**VERSION CONTROL**

**Question : What is the difference between git cherry-pick, git revert and git reset ? **

Answer : 
1. Git Reset (The Eraser) Use this command to go back in time and erase history. It moves your timeline pointer backward, making it look as though the deleted saves never happened.
>>>>>>> 8a56ca92f3c492f11351c4722d4d141a55ea1fd4

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
=======
