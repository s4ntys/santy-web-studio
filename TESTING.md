# Overenie projektu – 9. októbra 2026

Automatické funkčné testy v Chromium: **73 kontrol úspešných, 0 JavaScript chýb**.

- Všetkých 6 stránok: HTTP 200, hlavný nadpis, načítané lokálne fotografie.
- Desktop 1440 px a mobil 390 px: bez horizontálneho pretekania; funkčné mobilné menu.
- Autoservis: kalkulácia 35 + 45 = 80 €.
- Autoservis, reštaurácia, salón a barber: validné formuláre ukončia simuláciu s jasným upozornením, že skutočná rezervácia nevznikla.
- Reštaurácia: filter dezertov zobrazuje 2 jedlá; reset zobrazuje 6.
- Salón: výber Laury aktualizuje stylistu v rezervácii.
- Autodoplnky: vyhľadávanie, prázdny výsledok a kategórie.
- Košík: pridanie produktov, súčet 62 €, zníženie množstva na 38 €, odstránenie produktu na 24 €, ukončenie demo nákupu a zatvorenie Escape.
- Štúdio: výber balíka Business aktualizuje kontaktné zadanie; stiahnutie textového súboru funguje.
- Kontrola interných odkazov a súborov: všetky ciele existujú.
- Vizuálne skontrolovaný desktop hlavnej stránky a reštaurácie.

Testovanie prebehlo lokálne. Verejné nasadenie a jeho následný test zatiaľ neboli vykonané: Cloudflare login v Cloud Browseri zobrazuje chybu overenia a blokuje prihlásenie.

Pracovný e-mail štúdia nie je zadaný. Zatiaľ funguje stiahnutie zadania; po doplnení adresy do assets/config.js sa sprístupní e-mailový dopyt.
