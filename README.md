# Cod reducere Dormeo — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Dormeo** de pe [shopilo.ro](https://shopilo.ro/magazin/dormeo.ro). Returneaza **cupoane Dormeo** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-dormeo](https://shopilo-ro.github.io/cod-reducere-dormeo/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-dormeo
cd cod-reducere-dormeo
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Dormeo",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% reducere la saltele si lenjerii de pat",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/dormeo.ro"
  }
]
```

## Cupoane Dormeo disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 30% | 30% reducere la saltele si lenjerii de pat | [shopilo.ro](https://shopilo.ro/magazin/dormeo.ro) |

Codurile active: **[shopilo.ro/magazin/dormeo.ro](https://shopilo.ro/magazin/dormeo.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Dormeo?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/dormeo.ro), adauga produsele in cos pe Dormeo, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Dormeo?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Dormeo?
Pagina [shopilo.ro/magazin/dormeo.ro](https://shopilo.ro/magazin/dormeo.ro) este actualizata zilnic cu cele mai noi cod reducere Dormeo, voucher Dormeo si cupon promotional Dormeo.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Dormeo

Dormeo este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/dormeo.ro) cele mai bune cod reducere Dormeo, cupoane Dormeo verificate si voucher Dormeo active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-dormeo
```

```javascript
const { fetchCoupons } = require('cod-reducere-dormeo');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
