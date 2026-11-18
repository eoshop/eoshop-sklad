# EOSHOP Skladový skener v4

Nahraďte pouze `index.html` v repozitáři eoshop/eoshop-sklad, potvrďte Commit changes. Po publikaci otevřete https://eoshop.github.io/eoshop-sklad/?v=4 .

- Živý skener EAN: @zxing/browser (bez závislosti na nativním BarcodeDetector).
- Interní kód: volitelné OCR ze živého obrazu přes Tesseract.js, může být na mobilu pomalé nebo nepřesné.
- Uloží se pouze kódy a počet kusů, ne fotografie.
- EAN je povinný pro uložení produktu; interní kód není povinný.
- Historie je lokální v prohlížeči daného zařízení. Přístup k historii z PC zatím není implementován.
- Pro čtečku i OCR je nutný internet k načtení knihoven a HTTPS pro kameru.
- Pokud fotoaparát nereaguje, zkontrolujte oprávnění kamery v Safari a obnovte stránku.
