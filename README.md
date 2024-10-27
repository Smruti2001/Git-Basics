1. `git init` -> This powers your folder to be managed by git, and initialises a new repository. It also creates a .git folder that has all the relevant logic to manage versio of your project.

2. `Woking Area` -> There can be a bunch of files that are not currently handled by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in the Working Area is considered to be not in the staging area. When we do `git status` and we see a bunch of `untracked files` then these are actually calles to be in the working area.

3. `Staging Area` -> The staging area in Git is a space where changes are collected before they are committed to the repository. It acts as an intermediate step, allowing you to review and selectively commit changes. The staging area ensures that only the changes you intentionally add get committed, providing better control and organization over your project. It's like a clipboard that holds your changes until you're ready to officially save them.

4. `Repository Area` -> This area actually contains the details of all you previous registered version. And the files in this area, git already manages them and knows their version history.

5. `git add <file>` -> moves file from working area to staging area

6. `git rm --cached` <file> -> moves file back from staging area to working area

7. `commit` -> Commit is a particular version of the project. It captures a snapshot of the project's staged changes and creates a version out of it.

8. `git commit` -> registers staging changes to a commit.

9. `git log` -> list downs all the commits of the repository.

10. `git restore <file>` -> it removes all files changes from the staging area to be committed. This can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

11. `git restore --staged <file>` -> it removes file from changes from staging area to the working area. this only works if changes are in your staging area

12. Diff between `git rm` and `git restore`. `Ans`: if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area or staging area then we git restore.

13. `git diff commit1 commit2` -> gives the difference of all file changes between two commits

14. `git commit -m "<your commit message>` -> If we want to avoid opening a text editor like vim/nano to add commit message we can use this following command.

15. `git remote` -> list down all the remote connection names

16. `Remote connection` -> It helps you to link two git repositories for uploading and downloading changes from each otherwise

17. `git remote add <name of remote> <link of the remote>` : this command helps us to add a new link to the remote repo and give a name to it.

18. `git remote rm <name of remote>` : this command deletes a remote connection

19. `git remote rename <oldname> <newname>` : this command remanes the remote connection.

`Note`: The name of the remote connection is always used to establish communication between the repos.

### Recommended practice to do
    - make changes
    - git add <file>
    - git commit 
    - git pull
    - git push 