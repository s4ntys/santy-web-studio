# SanTy Web Studio

Responzívne slovenské portfólio s piatimi samostatnými interaktívnymi konceptmi. HTML, CSS a JavaScript bez build procesu a bez externých runtime závislostí.

Verejný web: https://s4ntys.github.io/santy-web-studio/
Kontakt: zubajsamuel@gmail.com

## Ukážky
- TORQ Garage: odhad ceny a simulácia objednania servisu.
- Oliva Trattoria: filtrovaný jedálny lístok a simulácia rezervácie stola.
- Élan Hair Atelier: výber stylistu a simulácia rezervácie.
- Apex Auto Supply: vyhľadávanie, kategórie a funkčný demo košík.
- Noir Barber Club: cenník a simulácia rezervácie.

Všetky koncepty sú fiktívne. Rezervácie a nákupy neposielajú údaje na server a nevytvárajú objednávky. Fotografie sú generované ilustračné vizuály. Produkty používajú ilustračnú kolekciu doplnkov.

## Kontakt
Formulár pripraví zadanie ako textový súbor alebo otvorí e-mailovú aplikáciu cez mailto. E-mail musí používateľ odoslať v aplikácii; web nemá server na odosielanie správ.

## Hosting
GitHub Pages: main branch, root folder. `.nojekyll` umožňuje priame publikovanie súborov. Projekt funguje aj na Cloudflare Pages bez buildu: výstupný priečinok `/`. `_headers` sa uplatňuje na Cloudflare, nie na GitHub Pages.

## Úpravy
`assets/config.js` obsahuje kontakt. `assets/style.css` obsahuje základné štýly, `assets/design.css` finálny dizajn. `assets/app.js` spravuje interakcie. Fotografie a lokálne písma sú v `assets/`. Písma DM Sans a Cormorant Garamond používajú SIL Open Font License; licencie sú pri písmach.

## Prístupnosť
Mobilné menu, klávesnicové ovládanie, preskočenie na obsah, popisy formulárov, viditeľný focus a rešpektovanie prefers-reduced-motion.
