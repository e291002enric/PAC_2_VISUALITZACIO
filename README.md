# PAC 2 — Visualització de Dades

Tres visualitzacions interactives desenvolupades amb D3.js i HTML/CSS per a la PAC 2 de l'assignatura de Visualització de Dades.

---

## 1. Treemap — Tots els Municipis de Catalunya (2025)

![Treemap Població Catalunya](screenshots/01_treemap.png)

Cada rectangle representa un municipi de Catalunya. La mida és proporcional a la seva població i els colors identifiquen la comarca. Inclou tooltip interactiu i llegenda de comarques.

| | |
|---|---|
| **Tècnica** | Treemap (algorisme squarified) |
| **Eina** | D3.js v7 |
| **Dataset** | Idescat — Padró Municipal d'Habitants 2025 |
| **Abast** | 947 municipis · 43 comarques · 8.124.126 hab. |
| **Fitxer** | [`visualitzacions/01_treemap_poblacio_catalunya.html`](visualitzacions/01_treemap_poblacio_catalunya.html) |

> **Font:** [Open Data Catalunya — Padró Municipal d'Habitants](https://analisi.transparenciacatalunya.cat/Demografia/Padro-municipal-d-habitants-per-sexe-i-grups-d-eda/b4rr-d25b) · Institut d'Estadística de Catalunya (Idescat)

---

## 2. Icon Chart — Medalles Olímpiques París 2024

![Icon Chart Medalles París 2024](screenshots/02_iconchart.png)

Gràfic de pictogrames (estil ISOTYPE) que mostra les medalles d'or, plata i bronze dels 10 països amb més medalles als Jocs Olímpics de París 2024. Cada icona representa una medalla; els colors distingeixen el tipus.

| | |
|---|---|
| **Tècnica** | Icon Chart / Pictograma (ISOTYPE) |
| **Eina** | HTML + CSS (sense llibreries externes) |
| **Dataset** | Taula de medalles final — París 2024 |
| **Abast** | Top 10 països · Or, Plata i Bronze |
| **Fitxer** | [`visualitzacions/02_iconchart_medalles_paris2024.html`](visualitzacions/02_iconchart_medalles_paris2024.html) |

> **Font:** [Wikipedia — 2024 Summer Olympics medal table](https://en.wikipedia.org/wiki/2024_Summer_Olympics_medal_table) · [Olympics.com](https://www.olympics.com/en/olympic-games/paris-2024/medals)

---

## 3. Marimekko — Mix d'Energia Elèctrica Europa 2023

![Marimekko Energia Europa](screenshots/03_marimekko.png)

Gràfic Marimekko (mosaic) on cada columna és un país europeu. L'**amplada** de la columna és proporcional a la generació total (TWh) i l'**alçada** de cada franja mostra el percentatge de cada font d'energia renovable. Tooltip interactiu i llegenda de fonts energètiques.

| | |
|---|---|
| **Tècnica** | Marimekko / Mosaic Chart |
| **Eina** | D3.js v7 |
| **Dataset** | Mix elèctric renovable per país (2023) |
| **Abast** | Alemanya, França, Espanya, Itàlia, Suècia, Polònia |
| **Fitxer** | [`visualitzacions/03_marimekko_energia_europa.html`](visualitzacions/03_marimekko_energia_europa.html) |

> **Fonts:** Fraunhofer ISE · RTE France · Red Eléctrica (REE) · Terna · Ember · Eurostat

---

## Estructura del projecte

```
├── visualitzacions/
│   ├── 01_treemap_poblacio_catalunya.html
│   ├── 02_iconchart_medalles_paris2024.html
│   └── 03_marimekko_energia_europa.html
├── datasets/
│   ├── treemap_poblacio_catalunya.csv
│   ├── iconchart_medalles_paris2024.csv
│   └── marimekko_energia_europa2023.csv
└── screenshots/
    ├── 01_treemap.png
    ├── 02_iconchart.png
    └── 03_marimekko.png
```

## Com executar

Obre qualsevol fitxer `.html` directament al navegador. Les visualitzacions amb D3.js (treemap i marimekko) carreguen les dades embegudes al propi fitxer, sense necessitat de servidor.

---

*Assignatura: Visualització de Dades — UOC · 2025*
