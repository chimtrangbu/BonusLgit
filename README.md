# Core Project
https://github.com/chimtrangbu/lgit/blob/master/README.md

# BONUS: branches
Notions: branching and merging
## Branches & merging
Branches are one of git's most powerful features. It allows developers to develop concurrent code, from one single point of code in time. This allows teams to work on different features separately.

Later on, when they are stable, those "branches" are merged into the main program.

For this bonus, you will implement the following commands:

- lgit branch: creates a new branch
- lgit checkout: replaces the working directory with the content of the head commit of the specified branch
- lgit merge: merges one branch onto another
- lgit stash: puts away in a "dirty working directory" the current changes, which allows to switch to a new branch without working files

To implement branches, you might have to modify a bit the structure of the .lgit directory. For example, it might be relevant to have a HEAD file pointing at the current branch. And it might be relevant to have a directory listing all existing branches. (For reference, git keeps track of those information in a directory called refs/heads. Look it up!)

Note: If you add some information to your commit objects (to include a reference to one or several parent commit objects maybe...?), be sure to respect the following structure:

- author name
- time of the commit
- 1 or several lines with additional information
- an empty line
- the commit message
