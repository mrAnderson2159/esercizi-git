# Esercizio 1 – Comandi Base: `init`, `status`, `add`, `commit`, `log`

## 🎯 Obiettivo

Esercitarsi con i comandi fondamentali di Git: inizializzare una repo, creare e modificare file, aggiungerli alla staging area, fare commit, e visualizzare la cronologia.

---

## 📋 Istruzioni

1. All'interno della cartella `esercizi-git`, crea una cartella chiamata `es-01` (questa!).
2. Crea un file chiamato `note.txt` e scrivici dentro una riga di testo qualsiasi.
3. Verifica lo stato della repo.
4. Aggiungi il file alla staging area.
5. Fai il primo commit con un messaggio significativo.
6. Modifica il file `note.txt` (aggiungi una seconda riga).
7. Verifica lo stato della repo dopo la modifica.
8. Aggiungi nuovamente il file alla staging area.
9. Fai un secondo commit.
10. Visualizza la cronologia dei commit con almeno due varianti del comando `git log`.

---

## 💡 Suggerimenti

- Usa `git status` prima e dopo ogni comando per vedere come cambia la situazione.
- Prova `git log`, `git log --oneline` e `git log --graph --oneline` per visualizzare la cronologia.
- Scrivi messaggi di commit descrittivi.

---

## ✍️ Comandi usati

In questa sezione puoi annotare i comandi che hai usato e cosa hanno fatto.

```bash
# Esempio
git status
git add note.txt
git commit -m "Aggiunto il file note.txt con contenuto iniziale"
