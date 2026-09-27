# Consegna Esercizio 12 — Riallineamento dopo modifica sul remoto

## Messaggio di errore ottenuto dal push
```text
PS F:\Users\samue\Documents\VsCode\Info-python\Python_Dallabrida_Samuele_4Bi> git push 
To https://github.com/SamueleDallabrida/Python_Dallabrida_Samuele_4Bi.git  ! [rejected]        main -> main (fetch first) 
error: failed to push some refs to 'https://github.com/SamueleDallabrida/Python_Dallabrida_Samuele_4Bi.git' 
hint: Updates were rejected because the remote contains work that you do not 
hint: have locally. This is usually caused by another repository pushing to 
hint: the same ref. If you want to integrate the remote changes, use 
hint: 'git pull' before pushing again. 
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

#### Comandi utilizzati per lo svolgimento:
- git pull
- git push
- git log --oneline --graph --decorate
- git add ...
- git commit ...

## Spiegazione in prosa del seguente esercizio

Il 'git push' in locale è stato rifiutato dato che il repository remoto, conteneva un commit  
(ossia la modifica al README) non registrato in locale.  
Git blocca l'invio e restituisce un errore anziche sovrascivere  
Eseguendo un git pull la versione locale viene aggiornata, e nel frattempo un merge fonde le 2 versioni, successivamente si effettua un git push per mandare  
tutte le modifiche al repository remoto  

#### Output del comando ***git log --oneline --graph --decorate***

* 0b810f3 (HEAD -> main, origin/main, origin/HEAD) fix(README.md): Modifica esercizio 12
* 3e43a0b fix(README.md): aggiunta comandi venv
* d0decba feat(recupero.md): Completamento esercizio 11 + file gitignore
* 672ae3b fix(ignore): rimossa cartella temporanei dal tracciamento
* bf0c298 test(env): aggiunti file temporanei per errore
* 59f0216 feat(README.md/cronologia.md): Completamento esercizio 9 - 10, con relativo readme.md nella cartella M0_ambiente
* 0c36887 feat(autenticazione.md): Completamento esercizio 8
* f14f5d4 feat(gitignore_verifica): Completamento esercizio 7
* 36abefd fix:(README.md): Linee testo sistemate
* a65f57b feat(README.md): Aggiunta esercizio 6 al file readme.md
* 264e7ce feat(Esercizio6):Completamento esercizio 6
* b9f22e9 feat(README.md): Aggiunta breve introduzione riguardante gli esercizi da 1 a 5
* adb5680 fix: Aggiunta commenti esplicativi agli esercizi svolti
* 160243b feat(configurazione_git.md): Completamento esercizio configurazione git


