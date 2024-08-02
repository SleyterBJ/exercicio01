@SleyterBJ ➜ /workspaces/codespaces-blank $ mkdir exercicio01
@SleyterBJ ➜ /workspaces/codespaces-blank $ cd exercicio01/
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 $ git init
Initialized empty Git repository in /workspaces/codespaces-blank/exercicio01/.git/

A)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt


B)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

        
C)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example - arquivo.txt"
[main (root-commit) f0e048b] git add example - arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log
commit f0e048b71481b186d2cc814d124e8be7c291aab7 (HEAD -> main)
Author: Sleyter Bispo <sleyterbispo@gmail.com>
Date:   Fri Aug 2 01:37:53 2024 +0000

    git add example - arquivo.txt


D)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt


E)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02


F)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

        
G)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff


H)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt 


I)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03


J)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore --staged arquivo.txt
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")

@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat arquivo.txt 
03


K)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example2 - arquivo.txt"
[main d2737b1] git add example2 - arquivo.txt
 1 file changed, 1 insertion(+), 1 deletion(-)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log
commit d2737b19b45d06475ef6d439d86b2aad0bf5a101 (HEAD -> main)
Author: Sleyter Bispo <sleyterbispo@gmail.com>
Date:   Fri Aug 2 01:42:02 2024 +0000

    git add example2 - arquivo.txt

commit f0e048b71481b186d2cc814d124e8be7c291aab7
Author: Sleyter Bispo <sleyterbispo@gmail.com>
Date:   Fri Aug 2 01:37:53 2024 +0000

    git add example - arquivo.txt

    
L)    
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore


M)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo "NOVO ARQ TXT" > novo.txt
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@SleyterBJ ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
