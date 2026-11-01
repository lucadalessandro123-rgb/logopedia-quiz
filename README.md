# La Logopedia di Luca

Quiz a crocette per materia, con login (Google o email) e progressi salvati per account.

- `index.html` – il sito
- `domande/<materia>.json` – le domande (anatomia, biologia, biochimica, fisica, statistica)
- `config.js` – configurazione del progetto Firebase
- `firestore.rules` – regole di accesso da incollare in Firebase > Firestore > Regole (elenco delle email autorizzate)

Ospitato con GitHub Pages; login e progressi con Firebase (piano gratuito Spark).

## Domande da non riproporre

Durante qualsiasi quiz il tasto «Non riproporre» toglie la domanda da tutti i quiz e dai conteggi e la sposta nella sezione «Domande da non riproporre» della pagina principale (divisa per materia e capitolo), da dove si può rimettere nei quiz. Sono salvate a parte in Firestore (`utenti/<uid>/escluse/<materia>`): azzerare i progressi non le tocca.
