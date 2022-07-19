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
