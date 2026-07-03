# Git Exercise Solutions

## Bundle 1

### Exercise 1

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git init
Initialized empty Git repository in /home/obed/Desktop/the-gym-git-exercise-solutions/.git/
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch -m master
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch -m main
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add README.md
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Create README.md file"
[main (root-commit) 0028d07] Create README.md file
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git remote add origin git@github.com:obedeveloper/the-gym-git-exercise-solutions.git
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 255 bytes | 127.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      main -> main
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch dev
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch dev
Switched to branch 'dev'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch test
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch test
Switched to branch 'test'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch dev
Switched to branch 'dev'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch -d test
Deleted branch test (was 0028d07).
```

### Exercise 2

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash
No local changes to save
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash -u
Saved working directory and index state WIP on dev: 0028d07 Create README.md file
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash -u
Saved working directory and index state WIP on dev: 0028d07 Create README.md file
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash -u
Saved working directory and index state WIP on dev: 0028d07 Create README.md file
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash list
stash@{0}: WIP on dev: 0028d07 Create README.md file
stash@{1}: WIP on dev: 0028d07 Create README.md file
stash@{2}: WIP on dev: 0028d07 Create README.md file
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash apply stash@{1}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash apply stash@{2}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add home and about pages"
[dev c4d4565] Add home and about pages
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 558 bytes | 279.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/dev
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      dev -> dev
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git stash pop
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped refs/stash@{0} (826536ce999d1105fef1dc32cae445e6c4f386c9)
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git restore .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git clean -fd
Removing team.html
```

## Bundle 2

### Exercise 1

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/bundle-2
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/bundle-2
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/bundle-2
```
