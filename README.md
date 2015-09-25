# git-toolbox
Repository for Fall 2015 Software Design - a toolbox exercise for learning more about using git

## Git Skills

** Basic **
- Check state of repository
- Add files
- Commits (and good format)
- Pushing

** Additional **
- Adding interactively
- Branching
- Merge conflicts?
- Editing previous commits - interactive rebase

## Practice basic skills

1. Fork this repository to your own GitHub account
2. Clone it to your local environment
3. Create a new file named `hello.py` and add a short Python program

### Notes on Commits
As you know, commits are a way to save a chunk of changes to your code at a specific point.  To this end, it's important to have good commit messages that tell you what changed about your code at each commit.

You can see previous commit messages by running the command:
```
git log
```
Which commit messages for this repository are informative?  Which are not?  

If you ever plan to contribute to open-source projects, you'll need your commit messages to be informative.  In general, that means you should rarely by using the -m flag: `git commit -m ""short commit message here"` because it doesn't allow a lot of information.

Typing `git commit` with no arguments will open up a text editor that you can type a more detailed commit into.  If you want to change the text editor it uses (TOTALLY optional), you can do so with the command:
``` $ git config --global core.editor neweditornamehere ```

In general, it's accepted in most coding communities that a commit message should take this general format:
```
<Section of code edited>: <Summary of changes made in present tense>

<Additional details of what changed>
```

All lines should be less than 80 characters long.  The additional details will probably be longer than this - you should manually press enter after about 80 characters to start a new line.

For example, as you saw when running `git log`, the second commit for this repository took this format:
```
Readme: Add some tasks regarding initial steps and commits

Took notes in the README to lay out an outline for this toolbox, and drafted
some initial steps for students to follow in cloning the repo and learning
about commits and commit messages.
```