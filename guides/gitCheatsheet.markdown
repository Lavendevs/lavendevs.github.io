---
layout: page
title: github cheatsheet
category: guides
---

basic operations:
Interacting with the remote repository (that thing you see when opening i. e. [lavendevs/lavendevs.github.io](https://github.com/lavendevs/lavendevs.github.io))
- ```git clone <repository>```: one of the development start points. Clone a repository like [lavendevs/lavendevs.github.io](https://github.com/lavendevs/lavendevs.github.io) to your local machine.
- ```git push```: pushes the committed changes to the remote repository
File Management:
- ```git add <file> [<file2>, <file3>,...]```: Adds a file to the repository.
- ```git rm <file> [<file2>, <file3>,...]```: Removes a file to the repository.
- ```git mv <file> [<file2>, <file3>,...] <target>```: Moves a file to the new target and notifies git about it. Git needs to know, it wont find it if moved otherwise.
Applying changes:
- ```git commit <file> [<file2>, <file3>,...] -m <message>``` / ```git commit -a -m <message>```: Commits (adds) the changes to the repository.
- ```git stash```: reverts all uncommitted changes

a bit more advanced (important for us):
Branches:
- ```git branch --list -a```: Lists all currently active branches of the repository
- ```git branch <branch>```: Creates new branch with specified name.
- ```git switch <remote> <branch>```: Switches to the specifies branch. remote is origin by default.
- ```git branch -d <branch>```: Deletes specified branch.

a bit more advanced (not that important for us):
Tags (specific labeled points in development, interesting i. e. for releases):
- ```git checkout <tag>```: Sets local state of development to the specified tag; checkout HEAD to go back to current state.
- ```git tag <tag>```: Creates a tag with specified name.
- ```git tag -d <tag>```: Deletes tag locally; requires next line if deletion is also intended for the remote repository
- ```git push origin :refs/tags/<tag>```: Deletes tag on the remote repository.
