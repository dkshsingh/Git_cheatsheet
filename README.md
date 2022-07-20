# Git_cheatsheet
## initializing a repository
```
$ git init
```
## 1.Staging files
#stage a single file
```
$ git add file1
```
#stage multiple files
```
$ git add file1 file2
```
#stage with pattern
```
$ git add *.js
```
#stage the current directory and all its content
```
$ git add .
```
## 2.Viewing the status
#full status
```
$ git status
```
#short status
```
$ git status -s
```
## 3. committing the staged files
#commits with a one-line message
```
$ git -m "message"
```
#opens the default editor to type a long message
```
$ git commit
```
## 4. Skipping the area
```
$ git commit -am "message"
```
## 5. removing the files
#removes from working directory and staging area
``` 
$ git rm file1
```
#removes from staging area only
```
$ git rm --cached file1
```
## 6. Renaming or moving files
```
$ git mv file1.js file2.txt
```
## 7. Viewing the staged/unstaged changes
#show unstaged changes
```
$ git diff
```
#show staged changes
```
$ git diff --staged
```
#same as the above
```
$ git diff --cached
```
## 8. Viewing the history
#full history
```
$ git log
```
#summary
```
$ git log --oneline
```
#lists the commits from the oldest to newest
```
$ git log --reverse
```
## 9. viewing a commit
#shows the given commit
```
$ git show 921a2ff
```
#show the last commit
```
$ git show HEAD
```
#two steps before the last commit
```
$ git show HEAD~2
```
#show the version of file1 sorted in the last commit
```
$ git show HEAD:file1
```
## 10. Unstaging files(undoing git add)
```
$ git restore --staged file1
```
## 11. discarding local changes
#copies file1 from index to working directory
```
$ git restore file1
```
#restores multiple file
```
$ git file1 file2
```
#discard all local changes
```
$ git restore
```
#removes all untracked file
```
$ git clean -fd
```
## 12. Restoring an earlier version of a file
```
$ git restore --source=HEAD~2 file1
```
## 13. Viewing the history
#shows the list of modified files
```
$ git log --stat
```
#shows the actual changes
```
$ git log --patch
```
## 14. Filtering the history
#shows the last 3 entries
```
$ git log -3
```
```
$ git log --author="Mosh"
$ git log --before="2020-08-17"
$ git log --after="one week ago"
```
#commit with "GUI"in their message
```
$ git log --grep="GUI"
```
#commit with GUI in their patches
```
$ git log -S"GUI"
```
#range of commits
```
$ git log hash1..hash2
```
#commit that touches
```
$ git log file.txt
```
## 15. Formatting the log output
```
$ git log--pretty=format:"%an committed %H"
```
## 16. Creating an alias
```
$ git config --global alias.lg"log --oneline"
```
## 17.Viewing a commit
``` 
$ git show HEAD~2
```
#shows the version of file stored in this commit
```
$ git show HEAD~2:file1.txt
```
## 18.Checking out a commit
#checks out the given commit
```
$ git checkout dad47ed
```
#checks out the master branch
```
$ git checkout master
```
## 19. Finding a bad commit
```
$ git bisect start
```
#marks the current commit as a bad commit
```
$ git bisect bad
```
#marks the current commit as a good commit
```
$ git bisect good ca49180
```
#treminates the bisect session
```
$ git bisect reset
```
## 20. Finding contributors
```
$ git shortlog
```
## 21. Viewing the history of file
#shows the commits that touches file.txt
```
$ git log file.txt
```
#shows statics (the number of changes) for file.txt
```
$ git log --stat file.txt
```
#shows the patches (changes) applied to file.txt
```
$ git log --patch file.txt
```
## 22. Finding the authors of lines
```
$ git blame file.txt
```
## 23. Tagging
#tags the last commit as vl.0
```
$ git tag vl.0
```
#tags an earlier commit
```
$ git tag vl.0 5e7a828
```
#list all the tags
```
$ git tag 
```
#deletes the given tag
```
$ git tag -d vl.0
```
