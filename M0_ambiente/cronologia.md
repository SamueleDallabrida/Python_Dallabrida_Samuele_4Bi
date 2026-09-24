# Esercizio 9 — Lettura e interpretazione della cronologia

## Output dei Comandi

### Output di `git log --oneline --graph --decorate`
* 0c36887 (HEAD -> main, origin/main, origin/HEAD) feat(autenticazione.md): Completamento esercizio 8  
* f14f5d4 feat(gitignore_verifica): Completamento esercizio 7  
* 36abefd fix:(README.md): Linee testo sistemate  
* a65f57b feat(README.md): Aggiunta esercizio 6 al file readme.md  
* 264e7ce feat(Esercizio6):Completamento esercizio 6  
* b9f22e9 feat(README.md): Aggiunta breve introduzione riguardante gli esercizi da 1 a 5  
* adb5680 fix: Aggiunta commenti esplicativi agli esercizi svolti  
* 160243b feat(configurazione_git.md): Completamento esercizio configurazione git  
* dbe52d0 feat(esecuzione.md): Completamento elenco comando usato in orario.py  
* aecd83c fix:Sintassi markdown comandi  
* 8157daa feat(orario.py): Svolto il programma richiesto nell'esercizio 3  
* 526765a fix(percorsi.md): correzione scaletta dei passaggi  
* d6af650 feat(versioni.md\percorsi.md): Completato esercizio1 e esercizio2 da finire  
* 8204e51 Initial commit  

### Output di `git log -5 --pretty=format:"%h %ad %an %s" --date=short`
0c36887 2026-09-24 Samuele Dallabrida feat(autenticazione.md): Completamento esercizio 8  
f14f5d4 2026-09-24 Samuele Dallabrida feat(gitignore_verifica): Completamento esercizio 7  
36abefd 2026-09-24 Samuele Dallabrida fix:(README.md): Linee testo sistemate  
a65f57b 2026-09-24 Samuele Dallabrida feat(README.md): Aggiunta esercizio 6 al file readme.md  
264e7ce 2026-09-18 Samuele Dallabrida feat(Esercizio6):Completamento esercizio 6  

## Commento sulla Cronologia

La cronologia dei commit:  
- Initial commit: commit di creazione repository  
- feat(versioni.md\percorsi.md) Completamento dell'esercizio 1 e 2 con il 2 ancora da completare  
- feat(orario.py) Completamento programma esercizio 3  
- feat(README.md) Aggiunta breve introduzione riguardante gli esercizi da 1 a 5  

Nell'output del comando sono presenti tre etichette fondamentali tra parentesi:   
HEAD, main e origin/main. 
L'etichetta HEAD indica il punto in cui ci si trova attualmente all'interno del repository; in questo caso punta al ramo locale main. 
L'etichetta origin/main rappresenta lo stato del ramo principale sul server di GitHub. 
Il fatto che tutte 3 le etichette siano comparse nell'ultimo commit dimostra che il VsCode locale è sincronizzato con il repository github