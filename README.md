# PDF FakturaSorterare – Diesel & Bensin

Ett fristående offline-HTML-program som sorterar PDF-fakturor efter diesel- och bensinförbrukning. Allt bearbetas lokalt i webbläsaren – inga filer laddas upp.

## Funktioner
- Dra & släpp flera PDF-fakturor samtidigt
- Automatisk kategorisering av diesel-, bensin- och Aspen-rader via redigerbara nyckelord
- Extraherar liter, belopp och datum automatiskt
- Märkning per rad (fordon/objekt, t.ex. ”Gräv 1”) med fritext + förslag på tidigare märkningar
- Summeringar och bränslekostnad per märkning (liter och kronor per kategori)
- Sorterbar tabell
- Manuell rättning av kategori per rad
- Export till CSV (Excel-vänligt, svenska decimaler)

## Användning
1. Ladda ner `pdf.min.js` och `pdf.worker.min.js` (pdf.js 3.11.174) och lägg dem i samma mapp som `index.html`
2. Öppna `index.html` i en modern webbläsare
3. Dra in dina PDF-fakturor och exportera resultatet till CSV

## Begränsningar
- Textbaserade PDF:er fungerar (de flesta e-fakturor); skannade PDF:er utan text kräver OCR och stöds ej
- Utan lokala pdf.js-filer används CDN som reserv (kräver internet första gången)
