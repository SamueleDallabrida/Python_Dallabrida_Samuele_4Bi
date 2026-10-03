# Confronto tra le Varianti di Markdown

| Costrutto | Markdown Originale | CommonMark | GitHub Flavored Markdown (GFM) |
| :--- | :---: | :---: | :---: |
| Blocchi di codice recintati | No | Sì | Sì |
| Tabelle | No | No | Sì |
| Caselle di spunta | No | No | Sì |
| Testo barrato | No | No | Sì |
| Collegamenti automatici | Parziale | Parziale | Sì |
| Note a piè di pagina | No | No | No |

## Esempi delle Estensioni di GFM

### Lista di controllo (Task List)
- [x] Installare il JDK 17
- [x] Configurare Git e le credenziali dell'account
- [ ] Creare la struttura delle cartelle di progetto
- [ ] Completare gli esercizi sulla sintassi Markdown
- [ ] Verificare il rendering dei file in Visual Studio Code
- [ ] Effettuare il commit e il push su GitHub

### Riferimento a versioni o note precedenti
Per compilare il codice si usava la vecchia versione ~~Java 8~~, mentre ora è richiesto l'uso di Java 17 LTS per tutti i moduli del corso.

### Collegamento Automatico (Autolink)
Per consultare la documentazione di GitHub Flavored Markdown è possibile visitare l'indirizzo https://github.github.com/gfm/ senza dover formattare il link.

## Scelta della Variante per il Corso

Per le consegne di questo corso conviene utilizzare la variante GitHub Flavored Markdown (GFM) in quanto garantisce la corretta resa visiva di elementi fondamentali per la documentazione tecnica  come tabelle, elenchi di attività e sintassi avanzata per il codice. Essendo il repository del corso ospitato su GitHub, l'uso di GFM assicura che quanto visualizzato nell'anteprima corrisponda  esattamente alla resa finale sulla piattaforma Web. Se questo stesso file viene aperto con uno strumento che supporta esclusivamente lo standard CommonMark puro, le tabelle, il testo barrato, i  collegamenti automatici estesi e le caselle di spunta non verranno interpretati correttamente e saranno mostrati come testo semplice non formattato.  
