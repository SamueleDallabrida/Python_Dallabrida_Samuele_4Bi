# Python_Dallabrida_Samuele_4Bi M0_ambiente

Repository corso di informatica (Python)

- Breve sintesi degli esercizi che saranno svolti nel M0:
  - Esercizio 1:  
    Verificare che i 3 strumenti per creare l'ambiente siano funzionanti  
    Comandi da eseguire:  
    ```py --version```  
    ```code --version```  
    ```git --version```  

    Output dei seguenti comandi scritto in versioni.md  


  - Esercizio 2:  
    Creare all'interno della cartella 'Documenti' una cartella chiamata 'esercizio-percorsi', con dentro 2 sottocartelle chiamate rispettivamente
    'dati' e 'risultati'  
    Spostarsi in 'dati' e raggiungere 'risultati' utilizzando un percorso relativo  

    Una volta raggiunta la cartella 'risultati' eseguire un Get-Location di quest'ultima  
    Output e comandi sono stati trascritti nel file percorsi.md  


  - Esercizio 3:  
    Creazione del il file M0_ambiente/orario.py inserendo il codice dell'esercizio con il nome e numero di postazione.  
    Eseguire lo script dal terminale (es. python orario.py).  
    Le informazioni relative all'output e ai comandi usati sono presenti nel file esecuzione.md.  


  - Esercizio 4:  
    Configurare Git: Imposta i 4 parametri globali: il nome, l'email dell'istituto (usata su GitHub), il ramo predefinito (main) e VS Code come  editor.  
    Eseguire la verifica dal terminale usando il comando: ```git config --list --show-origin```  
    L'Output e la relativa spiegazione dei comandi usati è presente sul file chiamato configurazione_git.md.  


  - Esercizio 5:  
    Creare il repository: Su GitHub creare un repository privato chiamato lab-info-4bi-cognome (vuoto, no README.md, no .gitingore) e aggiungere il docente tra i collaboratori.  
    Creare il README.md: Nel file inserire nome, classe, anno scolastico e lo scopo del repository.  
    Collegare ed inviare: Collegare la cartella locale al repository GitHub con git remote add origin ... e inviare le modifiche online usando git push -u origin main.  
    Verificare: Eseguendo git status il terminale deve confermare che l'albero di lavoro è pulito e allineato con origin/main.  

  - Esercizio 6:  
    Creare tutta la struttura di cartelle che verranno utilizzate per le consegne durante tutto l'anno.  
    Per non lasciare le cartelle vuote (git non le registra) inserire un file ```.gitkeept``` vuoto, in ciascuna delle cartelle inserire un file  README.md con il titolo del modulo.  

    Comando: ```git ls-files```  
    Output:  
    M0_ambiente/configurazione_git.md
    M0_ambiente/esecuzione.md
    M0_ambiente/orario.py
    M0_ambiente/percorsi.md
    M0_ambiente/versioni.md
    M1_markdown_jupyter/.gitkeep
    M1_markdown_jupyter/README.md
    M2_python_fondamenti/.gitkeep
    M2_python_fondamenti/README.md
    M3_strutture_dati/.gitkeep
    M3_strutture_dati/README.md
    M4_funzioni_moduli/.gitkeep
    M4_funzioni_moduli/README.md
    M5_file_eccezioni/.gitkeep
    M5_file_eccezioni/README.md
    M6_oggetti/.gitkeep
    M6_oggetti/README.md
    M8_concorrenza_rete/.gitkeep
    M8_concorrenza_rete/README.md
    README.md
  
  - Esercizio 7:
    creare un file .gitignore nella radice del repository personale per escludere:
    - cache di Python (__pycache__/, file .pyc)
    - ambienti virtuali (.venv/, venv/)
    - file di stato dei notebook (.ipynb_checkpoints)
    - file temporanei di Windows (Thumbs.db, ecc.)
    - Per verificare che le regole funzionino:
    - Creare un ambiente virtuale di prova nella cartella M0_ambiente
      
    ```py -3.12 -m venv M0_ambiente\.venv```  
      
    Controllare che Git lo ignori tramite:  
      
    ```git status```
    ```git check-ignore -v M0_ambiente/.venv/pyvenv.cfg```   

    Risultato atteso:  
    git status non deve mostrare la cartella .venv tra i file non tracciati.  
    git check-ignore -v deve indicare il file .gitignore, la riga e il pattern che ha causato l’esclusione.  

    Output atteso:  
    il file .gitignore  
    il file M0_ambiente/gitignore_verifica.md contenente l’output dei due comandi.  
  
  - Esercizio 8  
    Eseguire l'autenticazione verso Github usando la chiave SSH  
    Comando per generare la chiave : ```ssh-keygen -t ed25519 -C "samuele.dallabrida09@marconirovereto.it"```  // (creazione della chiave)(algoritmo per la creazione della chiave)(commento con relativa mail di github)
    Comando per la restituzione a schermo della chiave: ```Get-Content ~/.ssh/id_ed25519.pub```  // (prende e restituisce un  testo)(percorso della cartella nascosta)(file che contiene la chiave pubblica)
    Comando per autenticazione: ```ssh -T git@github.com``` //(attiva secure shell)(dice a github che stai eseguendo un test di autenticazione)(indirizzo connesione ssh)
  
  - Esercizio 9:  
    Commentare la cronologia dei propri commit, e spiegare ciò che contiene ciascun commit.  
    In aggiunta fare un breve testo in cui appunto di definisce lo scopo di ciascun commit e si spiega a cosa servono  
    le svarie etichette (HEAD, origin/main, main)  
  
  - Esercizio 10:

installare venv
.\.venv\Scripts\activate
pip install ipykernel



  
    

