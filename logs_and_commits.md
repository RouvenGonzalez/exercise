# **Logs and Commits**

## **Last 3 Logs**

```
Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
$ git log
commit 7ca7b76e45500f3b53d3ca2cbd9ae2f8dd3168d7 (HEAD -> feature/13-stage_and_commit, origin/feature/13-stage_and_commit)
Author: RouvenGonzalez <rouvengonzalez@gmail.com>
Date:   Wed Apr 1 15:00:46 2020 +0200

    fixed format

commit 2e73c9d5cc764493c2563e146964c750e1ec4bf0
Author: RouvenGonzalez <rouvengonzalez@gmail.com>
Date:   Wed Apr 1 14:52:31 2020 +0200

    #13 stage and commit is complete!

commit bbe4c9adb749baa292c86844561dfccdb3c93a88 (origin/develop, origin/HEAD, develop)
Author: Tai 'Mr. T' Truong <tai.truong@software-developer.org>
Date:   Mon Mar 30 21:13:05 2020 +0200

    new feature...
```


## **Log 3 Explained**

```
commit bbe4c9adb749baa292c86844561dfccdb3c93a88 (origin/develop, origin/HEAD, develop)
```
* **Shows Git ID and the origin/ HEAD branch**


```
Author: Tai 'Mr. T' Truong <tai.truong@software-developer.org>
Date:   Mon Mar 30 21:13:05 2020 +0200
```
* **Author information and date of the commit**


```
    new feature...
```
* **Commit message**

## **Log 3 Changes**

```
Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
$ git show bbe4c
commit bbe4c9adb749baa292c86844561dfccdb3c93a88 (origin/develop, origin/HEAD, develop)
Author: Tai 'Mr. T' Truong <tai.truong@software-developer.org>
Date:   Mon Mar 30 21:13:05 2020 +0200

    new feature...

diff --git a/myfile.md b/myfile.md
new file mode 100644
index 0000000..270c611
--- /dev/null
+++ b/myfile.md
@@ -0,0 +1 @@
+hello, world!
```


## **Log 2 Changes**

```
Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
$ git show 2e73c9
commit 2e73c9d5cc764493c2563e146964c750e1ec4bf0
Author: RouvenGonzalez <rouvengonzalez@gmail.com>
Date:   Wed Apr 1 14:52:31 2020 +0200

    #13 stage and commit is complete!

diff --git a/challenge-010/stage_and_commit.md b/challenge-010/stage_and_commit.md
new file mode 100644
index 0000000..a9f241d
--- /dev/null
+++ b/challenge-010/stage_and_commit.md
@@ -0,0 +1,263 @@
+# **Create New File**
+
+'''
+Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
+$ touch stage_and_commit.md
+
+Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
+$ git status
+On branch feature/13-stage_and_commit
+Your branch is up to date with 'origin/feature/13-stage_and_commit'.
+
+Untracked files:

Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)

```


## **Log 1 Changes**

```
Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
$ git show 7ca7b7
commit 7ca7b76e45500f3b53d3ca2cbd9ae2f8dd3168d7 (HEAD -> feature/13-stage_and_commit, origin/feature/13-stage_and_commit)
Author: RouvenGonzalez <rouvengonzalez@gmail.com>
Date:   Wed Apr 1 15:00:46 2020 +0200

    fixed format

diff --git a/challenge-010/stage_and_commit.md b/challenge-010/stage_and_commit.md
index a9f241d..2cf3947 100644
--- a/challenge-010/stage_and_commit.md
+++ b/challenge-010/stage_and_commit.md
@@ -80,24 +80,24 @@ index d3785e0..6d3a108 100644
 +++ b/challenge-010/stage_and_commit.md
 @@ -16,7 +16,7 @@ Untracked files:
  nothing added to commit but untracked files present (use "git add" to track)
- '''
+

 -**Stage Output**
 +## **Stage Output**

- '''
+
  Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
 @@ -32,7 +32,7 @@ Changes to be committed:
          new file:   stage_and_commit.md
- '''
+

 -**Diff**
 +## **Diff**

- '''
+
  Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
 @@ -40,3 +40,34 @@ $ git diff
- '''
+

  The git diff command shows nothing because it has no staged file too compare with.
 +
@@ -109,8 +109,8 @@ index d3785e0..6d3a108 100644
 +
 +## **Check Status**
 +
-+'''
-+'''
++
++
 +Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
 +$ git status
 +On branch feature/13-stage_and_commit
@@ -124,7 +124,7 @@ index d3785e0..6d3a108 100644
 +  (use "git add <file>..." to update what will be committed)
 +  (use "git restore <file>..." to discard changes in working directory)
 +        modified:   stage_and_commit.md
-+'''
++
 +
 +The status command now shows 2 versions of our file.
 +One is the staged version and the other one is the modified one that's not staged.
@@ -188,7 +188,7 @@ index caccaca..b18eb05 100644

 +## **Status after Staging**
 +
-+'''
++
 +Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
 +$ git status
 +On branch feature/13-stage_and_commit
@@ -197,7 +197,7 @@ index caccaca..b18eb05 100644
 +Changes to be committed:
 +  (use "git restore --staged <file>..." to unstage)
 +        new file:   stage_and_commit.md
-+'''
++
 +
 +now the staged file was updatet with the modifications so only one version of our file remains.
 +
@@ -215,7 +215,7 @@ odified one.

 +## **Status after Staging**
 +
-+'''
++
 +Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sa
 ndbox/challenge-010 (feature/13-stage_and_commit)
 +$ git status
@@ -225,7 +225,7 @@ ndbox/challenge-010 (feature/13-stage_and_commit)
 +Changes to be committed:
 +  (use "git restore --staged <file>..." to unstage)
 +        new file:   stage_and_commit.md
-+'''
++
 +
 +now the staged file was updatet with the modifications so only one version of our file remains.
 +
@@ -233,7 +233,7 @@ ndbox/challenge-010 (feature/13-stage_and_commit)
 +
 +## **Git Status**
 +
-+'''
++
 +Medion AKOYA@DESKTOP-76ECOJG MINGW64 ~/Desktop/Rouven/Programmieren/Gitspace/sandbox/challenge-010 (feature/13-stage_and_commit)
 +$ git status
 +On branch feature/13-stage_and_commit
@@ -247,7 +247,7 @@ ndbox/challenge-010 (feature/13-stage_and_commit)
 +  (use "git add <file>..." to update what will be committed)
 +  (use "git restore <file>..." to discard changes in working directory)
 +        modified:   stage_and_commit.md
-+'''
++
 +
 +Again a new modified version exists.

```

