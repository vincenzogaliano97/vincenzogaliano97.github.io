# Vincenzo Galiano — sito personale

Portfolio statico in italiano, pronto per GitHub Pages. Non richiede installazione o compilazione.

## Anteprima locale

Apri `index.html` nel browser, oppure avvia dalla cartella del progetto:

```sh
python -m http.server 8000
```

Apri quindi http://localhost:8000.

## Contenuti

- `index.html`: presentazione, competenze, esperienze e contatti.
- `style.css`: impaginazione responsive, colori e caratteri.
- `script.js`: menu mobile e anno nel footer.
- `assets/`: foto personale, font locali e favicon.

La foto e i font sono serviti direttamente dal sito. Nessuna dipendenza JavaScript esterna, tracciamento o form con invio dati.

## GitHub Pages

Nel repository `vincenzogaliano97.github.io`, configura **Settings → Pages → Deploy from a branch**, selezionando il branch che contiene i file e la cartella **/ (root)**. Dopo il push, GitHub Pages pubblicherà il sito su https://vincenzogaliano97.github.io/.
