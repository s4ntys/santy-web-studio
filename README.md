# SanTy Web Studio

Hotový statický projekt v HTML/CSS/JavaScripte. Bez build procesu a bez závislostí. Všetky fotografie sú originálne AI vizuály fiktívnych projektov.

## Stránky
- `/` – štúdio, portfólio, služby, orientačný cenník a zadanie projektu
- `/demos/autoservis/` – TORQ Garage; kalkulátor servisných prác a demo rezervácia
- `/demos/restauracia/` – OLIVA; filtrovanie menu a demo rezervácia stola
- `/demos/salon/` – ÉLAN; výber stylistu, služieb a termínu
- `/demos/autodoplnky/` – APEX; vyhľadávanie, kategórie, košík, množstvá a simulácia objednávky
- `/demos/barber/` – NOIR; služby, FAQ a demo rezervácia

Všetky demo prevádzky, služby, produkty a ceny sú fiktívne. Formuláre nevytvárajú reálne rezervácie ani objednávky. Platby sa nevykonávajú. Dáta sa neodosielajú a neukladajú do databázy. Košík sa pri obnovení stránky vymaže.

## Kontakt štúdia
Do `assets/config.js` doplňte potvrdený pracovný e-mail a prípadne telefón:

```js
window.STUDIO_CONFIG = { email: 'VAS_PRACOVNY_EMAIL', phone: '' };
```

Prázdny e-mail ponechá funkčné stiahnutie zadania projektu. Po doplnení adresy sa zobrazí tlačidlo, ktoré otvorí e-mailovú aplikáciu s pripraveným dopytom. Web sám e-mail neodosiela. Pred obchodným používaním potvrďte cenník a doplňte zákonom vyžadované identifikačné údaje podnikateľa podľa skutočného spôsobu podnikania.

## Lokálne spustenie
V priečinku projektu:

```sh
python -m http.server 8080
```

Potom otvorte `http://localhost:8080`. Nepotrebujete Node.js ani npm.

## Cloudflare Pages – Direct Upload
1. Prihláste sa do svojho Cloudflare účtu.
2. Otvorte Workers & Pages, vytvorte aplikáciu a vyberte Pages / Direct Upload (Upload assets).
3. Zadajte názov projektu, napríklad `santy-web-studio`, ak je dostupný.
4. Nahrajte dodaný ZIP. Jeho koreň obsahuje `index.html`, `assets` a `demos`.
5. Publikujte. Verejnú adresu prideľuje Cloudflare; názov aj URL treba potvrdiť z výsledku nasadenia.
6. Otestujte hlavnú stránku a všetkých päť ciest na verejnom webe.

Nevyžaduje sa build príkaz ani server. Pri Git integrácii zvoľte framework None, build príkaz nechajte prázdny a výstupný priečinok nastavte na koreň projektu. Aktualizácie pri Direct Upload vykonávajte nahratím celého nového ZIP cez Create deployment.

`_headers` obsahuje základné bezpečnostné hlavičky. `404.html` poskytuje vlastnú chybovú stránku. Nepoužíva sa analytika, externé fonty ani sledovacie cookies. Smerovanie dem je riešené samostatnými priečinkami s `index.html`.

Oficiálna dokumentácia: https://developers.cloudflare.com/pages/get-started/direct-upload/

## GitHub Pages – demo portfólio

Nahrajte index.html, assets/, demos/, 404.html a .nojekyll do koreňa verejného repozitára. V Settings → Pages vyberte Deploy from a branch, main, / (root), Save. Relatívne odkazy a assety fungujú aj pod cestou repozitára. GitHub Pages slúži na statické demo; neodosiela e-maily ani skutočné rezervácie. Bezpečnostné hlavičky zo súboru _headers sú podporované Cloudflare/Netlify, nie GitHub Pages.
