# SanTy Web Studio

Responzívne slovenské portfólio s piatimi samostatnými interaktívnymi konceptmi. HTML, CSS a JavaScript bez build procesu a bez externých runtime závislostí.

Verejný web: https://s4ntys.github.io/santy-web-studio/
Kontakt: zubajsamuel@gmail.com

## Päť samostatných dizajnov

Každé demo má vlastnú štruktúru HTML, navigáciu a súbor CSS. Zdieľa sa iba reset, formulárová prístupnosť, lokálne písma a funkčné simulácie.

## Ukážky
- TORQ Garage: servisný portál s bočnou navigáciou, kalkulátorom a objednaním v troch krokoch.
- Oliva Trattoria: fotografický úvod s prepínačom, jedálny lístok a rezervácia v modálnom okne.
- Élan Hair Atelier: módny magazín, lookbook, výber stylistu a rezervácia.
- Apex Auto Supply: obchodný katalóg, vyhľadávanie v hlavičke, kategórie v bočnom paneli a košík.
- Noir Barber Club: mestský plagátový dizajn, pohyblivý pás, rozbaľovacie služby a rezervačný panel.

Všetky koncepty sú fiktívne. Rezervácie a nákupy neposielajú údaje na server a nevytvárajú objednávky. Fotografie sú generované ilustračné vizuály. Produkty používajú ilustračnú kolekciu doplnkov.

## Kontakt
Formulár pripraví zadanie ako textový súbor alebo otvorí e-mailovú aplikáciu cez mailto. E-mail musí používateľ odoslať v aplikácii; web nemá server na odosielanie správ.

## Hosting
GitHub Pages: main branch, root folder. `.nojekyll` umožňuje priame publikovanie súborov. Projekt funguje aj na Cloudflare Pages bez buildu: výstupný priečinok `/`. `_headers` sa uplatňuje na Cloudflare, nie na GitHub Pages.

## Úpravy
`assets/config.js` obsahuje kontakt. `assets/style.css` obsahuje základné štýly, `assets/design.css` finálny dizajn. `assets/app.js` spravuje interakcie. Fotografie a lokálne písma sú v `assets/`. Písma DM Sans a Cormorant Garamond používajú SIL Open Font License; licencie sú pri písmach.

## Prístupnosť
Mobilné menu, klávesnicové ovládanie, preskočenie na obsah, popisy formulárov, viditeľný focus a rešpektovanie prefers-reduced-motion.
