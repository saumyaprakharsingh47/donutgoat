Devops -> DEV + OPS 

![alt text](image.png)

Code is the Dough and Build is the Bread 

----------------------------------------------
**VERSION CONTROL**

**Question : What is the difference between git cherry-pick, git revert and git reset ? **

Answer : 
1. Git Reset (The Eraser) Use this command to go back in time and erase history. It moves your timeline pointer backward, making it look as though the deleted saves never happened.

Analogy: Ripping a few faulty pages completely out of your diary.

Best For: Fixing local mistakes on your computer before sharing your work with anyone else.

2.Git Revert / "Reverse" (The Safe Undo)(Note: The actual command is git revert). Instead of deleting the past, it creates a brand-new commit that does the exact opposite of a faulty commit.

Analogy: Writing a new diary entry that says, "Ignore everything I wrote yesterday, it was a mistake."

Best For: Undoing an error on a shared public branch (like main) without messing up your team's commit history.

3. Git Cherry-Pick (The Copy-Paste)Use this command to grab a single specific commit from another branch and apply it directly onto your current branch. It does not move your timeline or delete anything.

Analogy: Seeing a great paragraph in someone else's book, photocopying it, and pasting it into your own book.

Best For: Snagging a specific bug fix or feature from a colleague's experimental branch without merging all their other work.

----------------------------------------------
