## — Navigazione e percorsi nel terminale

1. ```cd "Z:\Documenti"``` <!--Spostamento in documenti->
2. ```mkdir esercizio-percorsi``` <!--Creazione della cartella 'esercizio-percorsi'->
3. ```cd "Z:\Documenti\esercizio'percorsi"``` <!--Spostamento nella cartella 'esercizio-percorsi'->
4. ```mkdir dati``` <!--Creazione della cartella 'dati'->
5. ```mkdir risultati``` <!--Creazione della cartella 'risultati'->
6. ```cd "Z:\Documenti\esercizio'percorsi\dati"``` <!--Spostamento tramite percorso assoluto nella cartella dati->
7. ```cd ..\risultati``` <!--Spostamento tramite percorso relativo dalla cartella dati alla cartella risultati->
- Outpunt di ```Get-location``` <!--Comando che restituisce il percorso assoluto di un determinato file o cartella->
  -   
      ```PS Z:\Documenti\esercizio-percorsi\risultati> Get-Location
        Path
        ----
        Z:\Documenti\esercizio-percorsi\risultati```
