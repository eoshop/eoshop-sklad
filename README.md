# EOSHOP Skladový skener v9

Nahrajte `index.html` do repozitáře GitHub Pages místo původního souboru.

- Živá čtečka čárových kódů: ZXing Browser (vyžaduje internet a povolenou kameru).
- EAN má přednost před jiným kódem; textové kódy se aplikace pokusí vyčíst pomocí OCR po klepnutí na „Načíst štítek“.
- Interní kód EOSHOP je nepovinný. Počet kusů se zadává ručně.
- Dávky se ukládají do localStorage konkrétního prohlížeče; nejsou synchronizované mezi zařízeními.
- Excel lze stáhnout nebo sdílet přes systémovou nabídku iPhonu, pokud Safari podporuje sdílení souboru. Při nepodpoře se soubor stáhne.
- Snímky z kamery se neukládají.

Funkčnost je nutné otestovat na skutečném iPhonu a na vašich štítcích. OCR nemusí spolehlivě rozeznat každý typ produktového kódu.
