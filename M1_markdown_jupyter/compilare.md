## Esercizio 2:

1. Clonare il repository remoto ed entrare nella cartella del progetto appena creata:

    ```bash
    git clone [https://github.com/esempio/progetto-java.git]
    cd progetto-java
    ```

2. Verificare la struttura delle directory contenute nel progetto:
   - La cartella `src/` contiene tutti i file di codice sorgente Java.
   - La cartella `bin/` deve essere utilizzata per salvare i file `.class` compilati.

3. Creare la cartella `bin/` se non è già presente nel percorso di lavoro.

4. Compilare il file sorgente contenente il metodo `main` specificando l'opzione `-d`:

    ```bash
    javac -d bin/ src/MediaVoti.java
    ```

5. Eseguire l'applicazione appena compilata passando l'opportuno percorso alla classe `MediaVoti`:

    ```bash
    java -cp bin/ MediaVoti
    ```

> 'javac' is not recognized as an internal or external command, operable program or batch file.

In caso di questo errore, verificare che il JDK sia stato installato correttamente e che la variabile d'ambiente `PATH` includa il percorso della cartella `bin` del JDK.