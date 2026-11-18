# EOSHOP skladový skener – živé skenování

Nahraďte soubor `index.html` v repozitáři `eoshop/eoshop-sklad` tímto souborem. GitHub Pages: branch `main`, folder `/ (root)`.

- Mobilní kamera běží přímo na stránce, bez pořizování či ukládání fotografií.
- ZXing průběžně hledá EAN/UPC a další čárové kódy. Prohlížeč nemusí podporovat BarcodeDetector.
- Tlačítko „Načíst štítek“ provede jednorázové OCR snímku pouze v paměti a zkusí načíst interní kód. OCR může být pomalé nebo nepřesné; má časový limit 12 sekund a umožňuje ruční opravu.
- Uložení záznamu je rychlé, pouze kódy a množství do localStorage. Opakované EAN nejsou automaticky slučovány.
- Historie funguje **pouze na stejném zařízení a ve stejném prohlížeči**. Přístup z PC ke stejným záznamům vyžaduje budoucí integraci online databáze. Mazání dat prohlížeče odstraní lokální historii.
- Export XLSX a CSV. Všechny knihovny se načítají z CDN a vyžadují připojení k internetu při prvním načtení.
- Pokud jsou dva rozdílné přečtené EAN, zobrazí se varování. Jeden EAN není chyba.
