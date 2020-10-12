# Git Playground
## A place where I can break shit and try to fix them

This is my local git playground. Maybe I'll push it to github, maybe not...
    Clearly I pushed it so here it is.

## Adventure Log
### 11-Oct-2020

| Time  |   Description |
| --- | --- |
| 16:35 |   This file is created in github. Checking if this will successfully get pulled to my local repo. |
| 16:45 |   This edit is done in the local machine which is then `pushed` to the remote in github using `git push origin master`|
| 16:57 | Copied my own cheatsheet to this repo. About to attempt a longform `git pull` because the manual says "More precisely, git pull runs git fetch with the given parameters and calls git merge to merge teh retrieved branch heads into the current branch. With --rebase, it runs git rebase instead of git merge." So... next order of business is to find out what `git rebase` is all about. |
| 17:06 | Updated the README so it would contain the more verbose log that my commit messages supposedly are. Trying my hand on making tables in markdown, too because I haven't tried this before. |
| 17:27 | Can't make a proper table to save my life. Trying if this gets drawn properly. Also trying to push both the old local branch named feature0\_again and making a new branch called markdown where I can experiment with markdown before mergin it to the README.md because I can't follow simple syntax. |
| 17:31 | This edit lives in the branch named markdown, pushing this to remote next. |

### 12-Oct-2020
| Time | Description |
| --- | --- |
| 13:22 | If I push this to remote on another branch, changes will _not immediately_ reflect the README.md on my repo home... right? By the way I'm using `git push origin markdown` to push this to github. Not sure if this will work, honestly. |
| 15:35 | Just did that push and it did make another branch but also created a pull request saying how **I, the guy who made a pull request,** immediately wanted the branch to get merged with master. Next thing I'm going to check is what will happen if I straight up do another commit and push to the created markdown branch.
| 16:13 | Overhauled the git cheatsheet file and made it a markdown file with proper formatting and this is the part where I do the push these changes to the markdown branch after having specified the upstream branch to be `origin markdown` |
16:38 | I am trying to merge an old branch I renamed to `ancient-branch` to this current  `markdown` branch and it can't comprehend the differences between those because I've added a lot of shit here since so I'm deleting the <<<< HEAD up top and the ==== below this one retaining the "This is an ancient version of README.md" which I added while I was in the `ancient-branch` branch.
16:46 | I successfully added and committed the changes and checked the result of `git branch --merged` it acknowledged how I tried to merge `ancient-branch` to `markdown` doing another commit locally before pushing this to remote origin.

---
###### Here Lies The Remains of README.md From `ancient-branch` Now Gone
    This is my local git playground. Maybe I'll push it to github, maybe not.

    This is an ancient version of README.md
