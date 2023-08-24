# Git summary


1. git init
Used to initialize git repository
2. git add
Used to add file with changes to git staging area (middle phase before commit)
3. git status
Used to check if files have been changed and added to staging area
4. git commit -m
Used to make commit - add changes from working directory to repository. -m lets us add comment to commit, be sure to enclose text in single quotes
5. git push
Used to push local repository to online one on github. Be sure to add ''' -u origin master ''' when making first push. Master branch can be changed for Main
6. git remote add origin (URL)
Used to make a link between local and online repositories
7. git remote -v
Used to check if link has been completed
8. git log
Used to check previous commits
9. git commit --amend
To add additional file to commit or change commit message (add -m and message for this purpose)
10. git restore --staged <file>
Used to remove file from staged to unstaged area. If you add . instead of file name, all staged files will unstage
11. git reset --hard <commit hash>
Used to make file version same as when it was at chosen commit in repository
12. git restore <file>
Used to return file to a last committed state
13. git diff
Used to check differencies in file between current and last commited states. 
Shows differencies in modified files only, not staged. To check staged ones, add flag --staged.
You can add 2 hashes of commits to check difference between them.
14. echo 'text'
Used to print message in console.
If you add >> <file name>, text will be added to text file
If you add > <file name>, file will be rewritten with chosen text
15. .gitignore
You can create this file to ignore files while staging the whole folder.
All files (one for each line) in this file will not be staged.
This rules will only apply to new, untracked files.
'#' is used to add comment, will not affect ignoring.
'*' is used to ignore all files, you can type *.jpeg to ignore all .jpeg files or docs/*/tmp to ignore all tmp files in subfolders inside docs folder
'?' is similar to every symbol. You can use file?.txt to ignore file1.txt, file2.txt and so on.
[0-2] or [a-y] is used to add an array of symbols. file[0-3].txt will ignore file1, file2, file3, but not file4.
'/' will ignore only files in folder. /file for root directory, folder/ for all files in chosen directory.
'!' is used to invert rule. *.jpeg + !important.jpeg will exclude important.jpeg from rule.


