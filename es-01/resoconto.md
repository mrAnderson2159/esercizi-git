mr.alderson@192 esercizi-git % mkdir es-01

mr.alderson@192 esercizi-git % cd es-01 

mr.alderson@192 es-01 % touch README.md

mr.alderson@192 es-01 % nano README.md 

mr.alderson@192 es-01 % less README.md 

mr.alderson@192 es-01 % touch note.txt

mr.alderson@192 es-01 % nano note.txt 

mr.alderson@192 es-01 % cat note.txt 
Questa è senza alcun dubbio una riga di testo qualsiasi

mr.alderson@192 es-01 % git add note.txt 

mr.alderson@192 es-01 % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   note.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md


mr.alderson@192 es-01 % git add README.md 

mr.alderson@192 es-01 % git commit -m "Ho creato il file README.md e note.txt, dove ho inserito un messaggio significativo"
[main 5a900f1] Ho creato il file README.md e note.txt, dove ho inserito un messaggio significativo
 2 files changed, 41 insertions(+)
 create mode 100644 es-01/README.md
 create mode 100644 es-01/note.txt

mr.alderson@192 es-01 % nano note.txt 

mr.alderson@192 es-01 % cat note.txt 
Questa è senza alcun dubbio una riga di testo qualsiasi.
Ora voglio aggiungere una riga di testo molto più significativa della precedente!

mr.alderson@192 es-01 % git add note.txt 

mr.alderson@192 es-01 % git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   note.txt


mr.alderson@192 es-01 % git commit -m "Aggiunto testo ancora più importante a note.txt"
[main 57b1562] Aggiunto testo ancora più importante a note.txt
 1 file changed, 2 insertions(+), 1 deletion(-)

mr.alderson@192 es-01 % git log --oneline
57b1562 (HEAD -> main) Aggiunto testo ancora più importante a note.txt
5a900f1 Ho creato il file README.md e note.txt, dove ho inserito un messaggio significativo
d34c699 (origin/main, origin/HEAD) Initial commit

mr.alderson@192 es-01 % git log --stat   
commit 57b156252bb55825090af7e96b1fa48521cc4e67 (HEAD -> main)
Author: V. Molinari - mac <there.is.no.spoon.2159@gmail.com>
Date:   Tue Mar 18 17:04:31 2025 +0100

    Aggiunto testo ancora più importante a note.txt

 es-01/note.txt | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)

commit 5a900f1f4491edd3a8ba4a2f7061f0f2b5309b94
Author: V. Molinari - mac <there.is.no.spoon.2159@gmail.com>
Date:   Tue Mar 18 17:02:18 2025 +0100

    Ho creato il file README.md e note.txt, dove ho inserito un messaggio significativo

 es-01/README.md | 40 ++++++++++++++++++++++++++++++++++++++++
 es-01/note.txt  |  1 +
 2 files changed, 41 insertions(+)

commit d34c699195d3a0cc74f43805bc4e0bcfa50e499b (origin/main, origin/HEAD)
Author: mrAnderson2159 <44756705+mrAnderson2159@users.noreply.github.com>
Date:   Tue Mar 18 16:43:53 2025 +0100

    Initial commit

 README.md | 1 +
 1 file changed, 1 insertion(+)
