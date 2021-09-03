# Lesson Plan

## Concepts

- Setting up git
- What is version control?
- Basic git commands
- GitHub
- Pull requests
- Merge conflicts

## Intro

The learners will be exposed to git via the command line. We will be going through initializing a git project, commiting files to it, and pushing things to a remote repository (i.e. GitHub). Part 1 is meant to be a hands on experience with a lot of teacher guidance where as part 2 should allow the students to explore the concepts on their own with some leading questions from the teacher.

## Running the Lesson

### Installing git

Make sure students have git installing (`git --version`). If they don't, let them download it from the below link while you talk about version control. 
- http://git-scm.com/download/mac

### Version control

  - distributed version control
  - coordinates work between multiple devs
  - tracks who made what changes and when
  - revert back at any time
  - local and remote
  - "snapshots" of your code
  - this is done via commits

### Part 1: Git Basics

The following are steps to create a project inside of their CLI.

`git config`
  `git config --global user.name "Byron Mackay"`
  `git config --global user.email "byron.mackay@lambdaschool.com"`

`mkdir IntroToGit`
cd into it

`git init`

`touch README.md`

`git add/rm` (check `git status` to see the move)

`git commit` (modify a file _after_ commiting it)

`git remote`
  - create repository on github
  - add remote
    `git remote add origin <github repo url>`

`git push`
  - Add readme locally and push

`git branch` (add about_me.txt)
  `git branch about_me`
  `git checkout about_me`
  or
  `git checkout -b about_me`

`git merge` (merge about_me into main locally)
  `git merge about_me`

`git push` to remote

### Part 2: Pull Requests
- create github repo called "pull_request"
- Have all students pull the repo and create a branch
- Have everyone run the project (simple addition) and notice that the values do not add together (they subtract)
- have each student fix the code, commit, and push their changes up. Then have them create a PR.
- Find two solution that create a merge conflict (if none, make yourself)
- show that you can edit in GitHub
  - `git fetch`
  - `git status`
  - `git pull`

### Extension
- `git blame`
- `git rebase` (if you need to do this, get someone else to help you)
- .gitignore
- show that you can edit in GitHub
