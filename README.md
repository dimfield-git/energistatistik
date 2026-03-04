# Energistatistik

Ett enkelt verktyg för att analysera energiförbrukning i flerbostadshus och bostadsrättsföreningar.

Verktyget visualiserar och sammanställer **månatlig el- och värmeförbrukning** över flera år och ger en snabb överblick över energianvändning, variationer mellan år och total energibalans.

Applikationen körs helt i webbläsaren och kräver **ingen installation eller server**.

---

## Öppna verktyget

När GitHub Pages är aktiverat (Settings → Pages, Branch: `main`, Folder: `/root`) finns verktyget här:

**https://dimfield-git.github.io/energistatistik/**

---

## Funktioner

### Energigrafer
Verktyget ritar tre stapeldiagram:

- **Elförbrukning** (fastighetsel eller total el)
- **Värmeförbrukning** (fjärrvärme)
- **Total energiförbrukning**

Varje diagram visar:
- månad för månad
- flera år samtidigt
- staplar grupperade per månad (t.ex. Feb 2024 bredvid Feb 2025)

Det gör det enkelt att se exempelvis:
- om vintrar varit kallare
- om energibesparingar genomförts
- hur förbrukningen utvecklas över tid

---

### Årssummor
Under graferna visas en tabell med:
- årlig elförbrukning
- årlig värmeförbrukning
- total energianvändning
- förändring jämfört med föregående år

Detta ger en snabb **överblick över trender i energianvändningen**.

---

### Export av grafer
Varje diagram kan exporteras som **PNG-bild**.

Det gör det enkelt att använda graferna i:
- styrelsematerial
- energirapporter
- presentationer
- tekniska utredningar

---

## Inmatning av data

Energidata matas in **månad för månad**.

Du kan också **klistra in en kolumn direkt från Excel** (12/24/36/48/60 rader beroende på valt intervall). Verktyget klarar tusentalsavskiljare med mellanslag (t.ex. `62 970`).

Exempel (12 månader el):

```
62970
55768
60474
57296
56325
52468
54137
54708
56105
61615
60072
62162
```

Det går att mata in **1–5 år av data** i ett sammanhängande intervall.

---

## Primärenergital

Verktyget kan även beräkna **primärenergital enligt BBR** om följande uppgifter anges:
- Atemp
- geografisk justeringsfaktor (kommunbaserad tabell)
- ev. IMD-korrigering (om IMD är ikryssat)

Om uppgifter saknas visas graferna ändå, men primärenergitalet beräknas inte (visas som `—`).

---

## Typiska användningsområden

Verktyget är främst avsett för:
- styrelser i bostadsrättsföreningar  
- energikonsulter  
- energiingenjörer  
- fastighetsförvaltare  

Det lämpar sig särskilt för:
- uppföljning av energibesparingar  
- analys inför energideklaration  
- underlag till styrelsemöten  
- jämförelse mellan olika år

---

## Tekniskt

Applikationen är en **statisk HTML-sida** som körs lokalt i webbläsaren och använder Chart.js via CDN.

All beräkning sker lokalt. Ingen data skickas till någon server.

---

## Versioner

Tidigare versioner av verktyget finns i mappen:

```
/versioner
```

---

## Licens

Fri att använda inom föreningar, energiarbete och analys.
