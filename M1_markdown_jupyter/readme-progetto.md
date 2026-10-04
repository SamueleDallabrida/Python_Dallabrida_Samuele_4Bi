# MediaVoti

MediaVoti è un'applicazione Java da riga di comando sviluppata per leggere ed elaborare i voti degli studenti da un file CSV di ingresso.  
Il programma calcola automaticamente la media dei voti per ciascuna materia e genera un riepilogo dettagliato.  

## Requisiti di Sistema

| Componente | Requisito Minimo | Note |
| :--- | :--- | :--- |
| Sistema Operativo | Windows 10, macOS, Linux | Indipendente dalla piattaforma |
| Java Development Kit | JDK 17 o superiore | Necessario per la compilazione e l'esecuzione |
| Strumento di versione | Git 2.x | Opzionale, utile per clonare il repository |

## Installazione

1. Clonare il repository locale o scaricare i file:

    ```bash
    git clone [https://github.com/esempio/media-voti.git]
    cd media-voti
    ```

2. Creare la cartella di destinazione per i file compilati:

    ```bash
    mkdir -p bin
    ```

3. Compilare il codice sorgente sorgente utilizzando il compilatore Java:

    ```bash
    javac -d bin/ src/MediaVoti.java
    ```


### Formato del file di ingresso (`voti.csv`)

Il file di input deve essere salvato nella cartella principale del progetto, formattato in righe con i valori separati da virgole (Materia, Voto):

```text
Informatica,8.5
Sistemi e Reti,7.0
Matematica,6.5
Informatica,9.0
```

- Per eseguire l'applicazione e eseguire il file CSV, lanciare il comando specificando il percorso del file di input:
  - ```java -cp bin/ MediaVoti voti.csv````

### Output atteso:

--- RIEPILOGO VALUTAZIONI ---  
Materia: Informatica     | Media: 8.75  
Materia: Sistemi e Reti  | Media: 7.00  
Materia: Matematica      | Media: 6.50  
- - - - - - - - - - - - - - - - - - - 
Media Generale: 7.42  

### Struttura progetto:
media-voti/
├── bin/            # Cartella contenente i file .class compilati
├── src/            # Codice sorgente del progetto
│   └── MediaVoti.java
├── voti.csv        # File di dati di esempio
└── README.md       # Documentazione del progetto



