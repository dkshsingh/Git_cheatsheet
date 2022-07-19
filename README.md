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
