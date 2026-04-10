# Cod reducere Temu — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Temu** de pe [shopilo.it](https://shopilo.it/magazin/temu.com). Returneaza **cupoane Temu** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-temu](https://shopilo-it.github.io/codice-sconto-temu/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-temu
cd codice-sconto-temu
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Temu",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% di sconto per nuovi utenti",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/temu.com"
  }
]
```

## Cupoane Temu disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 30% | 30% di sconto per nuovi utenti | [shopilo.it](https://shopilo.it/magazin/temu.com) |

Codurile active: **[shopilo.it/magazin/temu.com](https://shopilo.it/magazin/temu.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Temu?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/temu.com), adauga produsele in cos pe Temu, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Temu?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Temu?
Pagina [shopilo.it/magazin/temu.com](https://shopilo.it/magazin/temu.com) este actualizata zilnic cu cele mai noi cod reducere Temu, voucher Temu si cupon promotional Temu.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Temu

Temu este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/temu.com) cele mai bune cod reducere Temu, cupoane Temu verificate si voucher Temu active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-temu
```

```javascript
const { fetchCoupons } = require('codice-sconto-temu');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
