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

### Exercise 2

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git pull origin main
From github.com:obedeveloper/the-gym-git-exercise-solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/service-redesign
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add our services listing"
[ft/service-redesign ff4a2c6] Add our services listing
 1 file changed, 6 insertions(+)
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 385 bytes | 385.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/ft/service-redesign
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch main
Switched to branch 'main'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add listing of our services"
[main 2a81f56] Add listing of our services
 1 file changed, 5 insertions(+)
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 377 bytes | 377.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
   b94a6b2..2a81f56  main -> main
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git diff main..ft/service-redesign
diff --git a/services.html b/services.html
index ec33712..e686668 100644
--- a/services.html
+++ b/services.html
@@ -8,9 +8,10 @@
   <body>
     <h1>Services</h1>

-    <ol>
-      <li>Xyz</li>
-      <li>Rst</li>
-    </ol>
+    <ul>
+      <li>Abcd</li>
+      <li>Opqr</li>
+      <li>Ijkl</li>
+    </ul>
   </body>
 </html>
```

## Bundle 3

### Exercise 1

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/team-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/team-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add team page"
[ft/team-page 3f167e7] Add team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 483 bytes | 120.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/ft/team-page
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      ft/team-page -> ft/team-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch main
Switched to branch 'main'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/contact-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/team-page
Switched to branch 'ft/team-page'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git log
commit 3f167e70d56f5c1b2975ace9ad46578b64e3dce4 (HEAD -> ft/team-page, origin/ft/team-page)
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Tue Jul 7 10:17:40 2026 +0200

    Add team page

commit a658341c1dc8efa8d6cdd7f393654f95bfcd7ce3 (origin/main, origin/HEAD, main, ft/contact-page)
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:57:28 2026 +0200

    Add solutions for exercise 2, bundle 2

commit 68411ef86c9aa76f2309acae0eabe390f75b351c
Merge: 2a81f56 799ef5b
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:52:49 2026 +0200

    Merge pull request #2 from obedeveloper/ft/service-redesign

    Add our services listing

commit 799ef5bb4ba8be8f17c4442cd6125ff7130f597f (origin/ft/service-redesign)
Merge: ff4a2c6 2a81f56
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:52:31 2026 +0200

    Merge branch 'main' into ft/service-redesign

commit 2a81f56976597ae330f1cf946690e41054d30c78
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:46:13 2026 +0200

    Add listing of our services

commit ff4a2c6c9ecfc905adfd50ee7af6aed16f56d068 (ft/service-redesign)
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:42:34 2026 +0200

    Add our services listing

commit b94a6b292634a96d42d377be01253f33452a06e8
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:38:37 2026 +0200

    Add solutions for exercise 1, bundle 2

commit c829d897cac55be2adc1e041bd10005e379dc5d0
Merge: 81e3d3d 4944e4d
Author: NIYOMUGISHA Obed <obed6@duck.com>
Date:   Fri Jul 3 08:23:58 2026 +0200

    Merge pull request #1 from obedeveloper/ft/bundle-2

obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/contact-page
Switched to branch 'ft/contact-page'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git cherry-pick 3f167e70d56f5c1b2975ace9ad46578b64e3dce4
[ft/contact-page 587cf4e] Add team page
 Date: Tue Jul 7 10:17:40 2026 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add contact page"
[ft/contact-page ec38d6b] Add contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 768 bytes | 128.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/ft/contact-page
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/faq-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/faq-page
Switched to branch 'ft/faq-page'
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add faq page"
[ft/faq-page eec2afd] Add faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 446 bytes | 148.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/ft/faq-page
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git revert 3f167e70d56f5c1b2975ace9ad46578b64e3dce4
[ft/faq-page eb18292] Revert "Add team page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 278 bytes | 139.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
   eec2afd..eb18292  ft/faq-page -> ft/faq-page
```

### Exercise 2

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/faq-page
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git branch ft/home-page-redesign
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch main
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add pricing page"
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git switch ft/home-page-redesign
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git rebase main
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git commit -m "Add price"
obed@obed-HP-EliteBook-840-G3:~/Desktop/the-gym-git-exercise-solutions$ git push origin ft/home-page-redesign
```

## Bundle 4

### Exercise 1

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git remote add git-copy git@github.com:obedeveloper/the-gym-git-exercise-solutions-copy.git
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git commit -m "Fix typo"
[main 229a479] Fix typo
 1 file changed, 1 insertion(+), 1 deletion(-)
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 366 bytes | 91.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
   352f495..229a479  main -> main
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git push git-copy main
Enumerating objects: 41, done.
Counting objects: 100% (41/41), done.
Delta compression using up to 4 threads
Compressing objects: 100% (37/37), done.
Writing objects: 100% (41/41), 8.47 KiB | 157.00 KiB/s, done.
Total 41 (delta 13), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (13/13), done.
To github.com:obedeveloper/the-gym-git-exercise-solutions-copy.git
 * [new branch]      main -> main
```

### Exercise 2

```bash
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git branch ft/footer
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git switch ft/footer
Switched to branch 'ft/footer'
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git commit -m "Add footer to the page"
[ft/footer ba01b4e] Add footer to the page
 1 file changed, 1 insertion(+)
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git add .
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git commit -m "Add copyright"
[ft/footer a7fa351] Add copyright
 1 file changed, 1 insertion(+), 1 deletion(-)
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 680 bytes | 170.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
   229a479..f1bc648  main -> main
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git push origin ft/footer
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 712 bytes | 118.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/ft/footer
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      ft/footer -> ft/footer
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git switch squashing
Switched to branch 'squashing'
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git merge --squash ft/footer
Updating f1bc648..a7fa351
Fast-forward
Squash commit -- not updating HEAD
 pricing.html | 1 +
 1 file changed, 1 insertion(+)
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git commit -m "Merge with squash"
[squashing 170e582] Merge with squash
 1 file changed, 1 insertion(+)
obed@obed-HP-EliteBook-840-G3:~/Desktop/The Gym/git$ git push origin squashing
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 407 bytes | 101.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'squashing' on GitHub by visiting:
remote:      https://github.com/obedeveloper/the-gym-git-exercise-solutions/pull/new/squashing
remote:
To github.com:obedeveloper/the-gym-git-exercise-solutions.git
 * [new branch]      squashing -> squashing
```
