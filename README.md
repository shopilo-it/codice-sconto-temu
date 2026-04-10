# Codice sconto Temu, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Temu** da [shopilo.it](https://shopilo.it/negozi/temu.com). Restituisce **coupon Temu** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-temu](https://shopilo-it.github.io/codice-sconto-temu/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-temu
cd codice-sconto-temu
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Temu",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% di sconto per nuovi utenti",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/temu.com"
  }
]
```

## Coupon Temu disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 30% | 30% di sconto per nuovi utenti | [shopilo.it](https://shopilo.it/negozi/temu.com) |

Codici attivi: **[shopilo.it/negozi/temu.com](https://shopilo.it/negozi/temu.com)**

## Domande frequenti

### Come utilizzo un codice sconto Temu?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/temu.com), aggiungi i prodotti al carrello su Temu e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Temu?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Temu piu recenti?
La pagina [shopilo.it/negozi/temu.com](https://shopilo.it/negozi/temu.com) viene aggiornata quotidianamente con i codici sconto Temu, voucher Temu e coupon promozionali Temu piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Temu

Temu e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/temu.com) trovi i migliori codici sconto Temu, coupon Temu verificati e voucher Temu attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-temu
```

```javascript
const { fetchCoupons } = require('codice-sconto-temu');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
