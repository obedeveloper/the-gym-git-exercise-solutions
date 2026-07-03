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
