# EOSHOP – Skladový EAN skener (prototyp)

## Nasazení na GitHub Pages
1. Na github.com vytvořte nové **Public** repository, např. `eoshop-sklad`.
2. Nahrajte soubor `index.html` do kořenového adresáře repozitáře (Add file → Upload files → Commit changes).
3. V Settings → Pages → Build and deployment zvolte Deploy from a branch, branch `main`, folder `/ (root)` a uložte.
4. Otevřete adresu `https://UZIVATEL.github.io/eoshop-sklad/` přes HTTPS, na mobilu povolte fotoaparát.

## Co prototyp umí
- Povinný název dávky před focením
- Fotoaparát telefonu, foto → ruční počet kusů → uložit a další
- Pokus o automatické načtení EAN pomocí BarcodeDetector a interního kódu pomocí OCR (Tesseract.js)
- Neshoda pouze při dvou různých načtených EAN
- Úprava načtených údajů, přehled výsledků, XLSX a CSV export
- Historie a fotografie uložené lokálně v IndexedDB prohlížeče

## DŮLEŽITÁ omezení
- **Mobil a PC zatím nemají společnou historii.** Pro synchronizaci je potřeba přidat cloudovou databázi (např. Supabase), autentizaci a pravidla přístupu. Nesdělujte do veřejného GitHub repozitáře tajné klíče.
- Rozpoznávání interních kódů z fotek pomocí OCR není stoprocentní. Vždy kontrolujte výsledky.
- BarcodeDetector není podporován ve všech prohlížečích. V takovém případě se lze opřít o OCR nebo údaje doplnit ručně.
- Knihovny OCR a Excel se načítají z veřejných CDN; při prvním použití je potřeba připojení k internetu.
- Lokální data se mohou ztratit po vymazání dat prohlížeče, změně telefonu či použití anonymního režimu. Průběžně exportujte.
- Aplikace je funkční prototyp, ne hotový firemní systém. Před ostrým nasazením je třeba otestovat mobilní fotoaparát, typy štítků, ukládání a obnovu.
