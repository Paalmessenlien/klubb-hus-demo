# klubb-hus-demo

Klikkbar demo av **Min side** for Lillehammer Bueskytterklubb (LBSK): hjem, aktivitet, hus (klubbspillet) og profil, med mockdata for fire medlemmer.

**Live:** https://paalmessenlien.github.io/klubb-hus-demo/

## Filer

| Fil | Innhold |
| --- | --- |
| `index.html` | Inngang. Monterer `Main` i full bredde. |
| `Main.dc.html` | Selve appen (markup, styling, mockdata og logikk). Responsiv: sidemeny fra 900 px, tabbar under. |
| `Mobil.dc.html` | Mobilvisning (390 px), brukt som artboard i designet. |
| `support.js` | Kjøretid for Design Component-formatet (`x-dc`, `sc-for`, `DCLogic`). |

Alt er statisk HTML/JS uten byggesteg. Test lokalt med `python3 -m http.server` og åpne `http://localhost:8000/`.
(Åpne via en server, ikke `file://`, fordi `Main` hentes med `fetch`.)

## Publisering

GitHub Actions (`.github/workflows/pages.yml`) publiserer til GitHub Pages ved hver push til `main`.
