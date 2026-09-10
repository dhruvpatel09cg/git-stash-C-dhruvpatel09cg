Q1: How many stashes? Which one is latest?

-->Answer:   
    There were two stashes in which 'stash@{0}: On main: WIP: temp.txt' is the latest stash.

Q2: Which stash has temp.txt?

-->Answer:   
    The latest stash stash@{0}: On main: WIP: temp.txt has temp.txt

Q3: What changed in the stash list after pop?

-->Answer:   
    After using pop the latest stash was transferred to working directory from stash stack and also the stash is removed from stash list.

Q4: What is git stash and why is it useful?

-->Answer:   
     git stash is a git command which provides temporary storage for uncommited changes allowing us to switch branches and make changes on different files without risk of losing these uncommited files. We may later bring back files from stash stack(temporary storage).

Q5: Explain with a small example:

-git stash apply
-git stash pop

-->Answer:

    git stash apply is like taking a copy of a document to use at a place while keeping original document saved
    so it can be used at different place in future.

    git stash pop is like giving original copy of any document at a place, it can't be used again once it get submitted at one place.

Q6: Why should we use -u when stashing new files?

-->Answer

    We should use -u while stashing new files if we want to include untracked files to the stash stack.

Q7: Why are meaningful stash messages (like "WIP: login form") important in team projects?

-->Answer

    Meaningful stash messages are very important in team projects as it provides clarity about files saved 
    in that stash making it easy to understand for other team members.

Q8: Imagine:

-You stashed 3 times.
-You run git stash pop.
-Then you run git stash drop.

How many stashes remain if you started with 3? Explain briefly

-->Answer

    Only one stash will remain after using git stash pop and git stash drop as pop transfer file to Working Directory and deletes the stash and drop deletes the stash without providing it on Working Directory.