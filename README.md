# Codice sconto Notino, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Notino** da [shopilo.it](https://shopilo.it/negozi/notino.it). Restituisce **coupon Notino** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-notino](https://shopilo-it.github.io/codice-sconto-notino/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-notino
cd codice-sconto-notino
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Notino",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su profumi e cosmetici",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/notino.it"
  }
]
```

## Coupon Notino disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su profumi e cosmetici | [shopilo.it](https://shopilo.it/negozi/notino.it) |

Codici attivi: **[shopilo.it/negozi/notino.it](https://shopilo.it/negozi/notino.it)**

## Domande frequenti

### Come utilizzo un codice sconto Notino?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/notino.it), aggiungi i prodotti al carrello su Notino e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Notino?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Notino piu recenti?
La pagina [shopilo.it/negozi/notino.it](https://shopilo.it/negozi/notino.it) viene aggiornata quotidianamente con i codici sconto Notino, voucher Notino e coupon promozionali Notino piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Notino

Notino e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/notino.it) trovi i migliori codici sconto Notino, coupon Notino verificati e voucher Notino attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-notino
```

```javascript
const { fetchCoupons } = require('codice-sconto-notino');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
