# Procedura di configurazione della postazione di lavoro Windows

- Guida che descrive i vari passaggi su come riconfigurare il proprio ambiente di lavoro git, su una macchina Windows appena ripristinata.

## Verifica ambiente e percorso

Comandi (bash):  
- ```git --version```
- ```echo $HOME```

Output:  
git version 2.x.x  
/c/Users/nome_utente (o percorso equivalente della home utente)  

## Configurazione identità di git

Comandi (bash):
- ```git config --global user.name "Nome Cognome"```
- ```git config --global user.email "utente@scuola.it"```

Controllo di verifica:
- ```git config --global --list```

Output:
user.name=Nome Cognome
user.email=utente@scuola.it

## Generazione o configurazione della chiave ssh

Comandi:
- ```ssh-keygen -t ed25519 -C "utente@scuola.it"```

Premere invio a tutte le seguenti proposte.  
Successivamente prendere e copiare la chiave ssh negli appunti e collegarla a github -> Settings (Profilo) -> SSH and GPG keys  
La chiave ssh si può ottenere tramite questo comando:  
- ```Get-Content $HOME/.ssh/id_ed25519.pub```

Controllo verifica:
- ```ssh -T git@github.com```

Output:
Hi 'username'! You've successfully authenticated, but GitHub does not provide shell access.  

## Clonazione del repository di lavoro

Comandi:
- ```cd $HOME/Documents``` //Spostamento nella cartella documenti dell'utente  
- ```git clone git@github.com:organizzazione/repository.git``` //Clonazione repository nella cartella  
- cd repository //Spostamento nella cartella del repository  

Controllo di verifica:   
- ```git status```

Output atteso:  
```text
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
```

## Risoluzione dei più comuni messaggi d'errore

### Errore 1: `git: 'psoh' is not a git command. See 'git --help'.`
- **Causa:** Errore di battitura durante l'inserimento di un comando Git (es. `git psoh` invece di `git push`).
- **Rimedio:** Riscrivere il comando con la sintassi corretta (`git push`).

### Errore 2: ```Permission denied (publickey)```
  - **Causa:****** La chiave SSH non è stata registrata sull'account GitHub oppure l'agente SSH non la trova nella cartella $HOME/.ssh.
  - **Rimedio:****************** Verificare la presenza del file $HOME/.ssh/id_ed25519.pub, copiarne il contenuto e aggiungerlo nelle impostazioni SSH del proprio profilo GitHub.

### Errore 3: ```fatal: not a git repository (or any of the parent directories): .git```
  - **Causa:** Si sta tentando di eseguire un comando Git (es. git status o git add) da una cartella che non è un repository Git.
  - **Rimedio:** Navigare nella cartella corretta del progetto clonata in precedenza usando cd $HOME/percorso/al/repo.

### Errore 4: ```! [rejected] main -> main (non-fast-forward)```
  - **Causa:** Il repository remoto contiene commit non presenti nella copia locale.
  - **Rimedio:** Eseguire git pull per integrare le modifiche remote prima di eseguire nuovamente git push.


