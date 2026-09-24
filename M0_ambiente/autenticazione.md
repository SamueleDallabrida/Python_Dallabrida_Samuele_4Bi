# Autenticazione verso GitHub

## Metodo Scelto
Chiave SSH (`id_ed25519`).

## Motivazione
Ho scelto l'autenticazione tramite chiave SSH dato che sto lavorando al mio pc personale di casa. Questo metodo mi permette di collegare permanentemente il mio PC al mio account GitHub, evitando di dover inserire credenziali o gestire token ad ogni operazione.

## Esito della Verifica
Comando eseguito:
`ssh -T git@github.com`

Output ottenuto:
`Hi SamueleDallabrida! You've successfully authenticated, but GitHub does not provide shell access.`