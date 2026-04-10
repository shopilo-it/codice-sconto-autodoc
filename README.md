# Codice sconto Autodoc, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Autodoc** da [shopilo.it](https://shopilo.it/negozi/auto-doc.it). Restituisce **coupon Autodoc** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-autodoc](https://shopilo-it.github.io/codice-sconto-autodoc/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-autodoc
cd codice-sconto-autodoc
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Autodoc",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su ricambi auto",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/auto-doc.it"
  }
]
```

## Coupon Autodoc disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su ricambi auto | [shopilo.it](https://shopilo.it/negozi/auto-doc.it) |

Codici attivi: **[shopilo.it/negozi/auto-doc.it](https://shopilo.it/negozi/auto-doc.it)**

## Domande frequenti

### Come utilizzo un codice sconto Autodoc?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/auto-doc.it), aggiungi i prodotti al carrello su Autodoc e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Autodoc?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Autodoc piu recenti?
La pagina [shopilo.it/negozi/auto-doc.it](https://shopilo.it/negozi/auto-doc.it) viene aggiornata quotidianamente con i codici sconto Autodoc, voucher Autodoc e coupon promozionali Autodoc piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Autodoc

Autodoc e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/auto-doc.it) trovi i migliori codici sconto Autodoc, coupon Autodoc verificati e voucher Autodoc attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-autodoc
```

```javascript
const { fetchCoupons } = require('codice-sconto-autodoc');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
