# Maricica învață să fie curată

**Poveste 3D interactivă în limba română, pentru copii de aproximativ 3 ani.**

Aplicație realizată cu HTML, CSS și JavaScript, fără framework, server sau cont de utilizator. Poate fi găzduită gratuit pe GitHub Pages. Conține cele 55 de înregistrări audio ale poveștii și 19 înregistrări pentru jocul de după poveste și păstrează același personaj Maricica în toate cele șase momente.

## Ce conține

- **Ascultă povestea:** înregistrări audio cu mai multe voci, subtitrare sincronizată pe fragmente, 6 momente, controale pentru pauză, repetare și navigare.
- **Povestește și joacă-te:** aceeași poveste, cu 5 opriri interactive. Copilul alege între două imagini mari și primește feedback prietenos.
- **Ne jucăm cu Maricica! (NOU):** 3 întrebări cu audio ElevenLabs, așteptarea atingerii răspunsului, voce de felicitare doar DUPĂ alegere, încurajare la răspuns greșit, 4 sarcini de mișcare cu pauze automate după terminarea instrucțiunii (6, 8, 7 și 8 secunde), opțiunea +5 secunde sau Gata, mai departe, apoi încheierea audio.
- **Alte jocuri:** alegerea obiectelor de igienă, ordonarea pașilor și descoperirea vocilor personajelor din înregistrările originale.
- **Pentru educatoare:** obiective didactice și recomandări de utilizare.

Audio-ul poveștii funcționează fără ElevenLabs sau alte servicii online: fișierele MP3 sunt în acest proiect. Pentru întrebările interactive, aplicația folosește *opțional* o voce românească instalată în browser/sistem. În lipsa ei, întrebările se afișează cu text și imagini, putând fi citite de educatoare.

## Publicare pe GitHub Pages

1. Creează un repository nou pe GitHub, de exemplu `maricica-interactiva`, cu vizibilitatea dorită pentru GitHub Pages.
2. Dezarhivează ZIP-ul și **încarcă în rădăcina repository-ului conținutul folderului `maricica-premium`**, nu doar fișierul ZIP. `index.html` trebuie să fie direct în rădăcină.
3. Accesează **Settings → Pages → Build and deployment → Deploy from a branch**.
4. Selectează **main** și **/(root)**, apoi salvează.
5. După publicare, accesează linkul indicat în pagina **Settings → Pages**.

Nu e nevoie de `npm install`, compilare, tokenuri API sau chei ElevenLabs.

## Testare înainte de activitatea cu copiii

- Verifică în Chrome/Edge pe tablă și pe telefon dacă sunetul pornește după apăsarea butonului „Ascultă povestea”. Browserul poate bloca pornirea automată a sunetului până la primul gest al utilizatorului.
- Parcurge fiecare din cele 6 momente și verifică funcționarea butoanelor înainte, înapoi, pauză și repetare.
- Testează toate cele 5 întrebări, jocul de ordonare și toate cele 4 obiecte din „Descopăr vocile”.
- Pe tabla Samsung, verifică dacă Maricica, întrebările și butoanele rămân în zona vizibilă.
- Dacă vei publica proiectul public, verifică drepturile de distribuire pentru înregistrările ElevenLabs și condițiile aplicabile adaptării operei literare.

## Structura

```text
maricica-premium/
├── index.html
├── style.css
├── script.js
├── favicon.svg
├── README.md
├── audio/
│   ├── 01.mp3
│   ├── ...
│   ├── 55.mp3
│   └── interactive/01.mp3 ... 19.mp3
└── assets/
    ├── maricica.webp
    ├── scenes/      (6 decoruri ilustrate, SVG)
    └── objects/     (9 obiecte/personaje, SVG)
```

## Aspecte educaționale și de confidențialitate

Conținutul este o adaptare pentru copii de 3 ani după **„Maricica” de Luiza Vlădescu**. Nu colectează date, nu afișează reclame și nu cere autentificare. Întrebările sunt pozitive și fără penalizări. Nu există contorizarea performanței copiilor.

## Notă despre personaj

Fișierul `assets/maricica.webp` conține **decupajul personajului ales de utilizatoare** din referința vizuală „Stil 1 – 3D (cartoon modern)”. Este reutilizat în toate scenele tocmai pentru a evita schimbarea fizionomiei. Mișcările sunt efecte 2D subtile și **nu** reprezintă animație 3D complexă, cu schelet articulat.

## Înregistrări ElevenLabs pentru jocul ghidat

Arhiva „ElevenLabs_Untitled_project.zip” a fost integrată în `audio/interactive/`, în ordinea celor 19 paragrafe exportate. Nu este necesară o nouă generare. Asocierea propusă, pe baza ordinii și a textului din conversație, este:

- 01–03: introducere; 04/05: întrebare și răspuns – mâini; 06/07: dinți; 08/09: pieptene.
- 10: invitație la mișcare; 11: arată mâinile; 12: mimează spălatul; 13: pieptănatul; 14: periajul.
- 15–18: felicitări/încheiere; 19: încurajarea „Mai încearcă o dată!”.

**Verificare recomandată:** fragmentele sunt exportate cu numere, fără transcrieri; ascultă succesiunea completă înainte de folosirea la grupă și confirmă că audio #19 este încurajarea. Temporizarea poate fi modificată din `GUIDED_MOTIONS[].seconds` în `script.js`.

Pauza începe doar **după terminarea fiecărei instrucțiuni**. Pauzarea aplicației oprește și numărătoarea inversă.
