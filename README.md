# Git Practice Project Task Two

This is a the implementation for a number guessing game.

## Purpose

Use this project to practice:
- Initializing a Git repository
- Creating and switching branches
- Making commits
- Merging branches
- Resolving merge conflicts

## Branch Structure

- main - Master branch that contains the stable, merged project
- dev - Contains development changes and messages for players
- feature1 - Implements quit feature, improved feedback messages for guesses, and play-again loop functionality
- feature2 - Implements max attempts logic and game over conditions
- feature3 - Includes bug fixes
- hotfix - Resolves issue with number generation
- documentation - Contains project documentation

## Learning Summary

### Differences between merge, rebase, squash, and cherry-pick

Merge takes a branch and integrates it into a new branch, usually the main or master branch.  
Rebase moves your branch's starting point to the tip of another branch.  
Squash is used during merging or rebasing to clean up commits.  
Cherry-pick allows you to apply a specific commit to your current branch rather than the entire branch that commit is on.  

### When you would use each strategy in real projects

Merge is used to integrate completed features implemented on a branch.  
Rebase is used to keep your keep your branch up to date with developments so the commit history is linear.  
Squash cleans up unorganized or unneeded commits and would be used when the history needs to be clean and readable.  
Cherry-pick is used to apply a simple bug fix without updating an entire branch.  

### What you observed in the git history for feature1 vs feature2 vs feature3

feature1 had minimal conflicts and was simple to merge.  
feature2 had 3 separate rebases. It required more merge conflict resolutions. I also ran into an issue here because I committed my changes before running gradle to ensure my code worked. I had to go back and fix a compile error and also adjust one of my output messages to pass the mathcing user test.  
feature3 had a messy commit history. This is when we used squash.  
