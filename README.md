# Maricica învață să fie curată — ediția 4.0 (poveste și jocuri)

Aplicație educațională pentru grupa mică (3 ani), adaptare după povestea „Maricica” de Luiza Vlădescu.

## Noutăți față de ediția Cinema 3D

- Scene vizuale mai detaliate pentru dormitor, baie, grădiniță și îngrijire. **Colega și ceilalți copii** sunt integrați într-o scenă 3D de grădiniță, nu imagini SVG separate.
- Imagine de baie cu Maricica în fața oglinzii și o **reflexie a modelului ales**; obiectele de igienă sunt mărite.
- Maricica este reprezentată cu urme discrete de murdărie înainte de spălare și curată după îngrijire.
- Puzzle cu **4 piese mari** (2×2). Copilul atinge piesa și locul ei. Nu este nevoie de drag-and-drop.
- Memory cu **două perechi** (patru cartonașe), fără cronometru și fără punctaj negativ.
- Păstrează jocul audio ElevenLabs cu cele 3 întrebări și 4 mișcări, pauze de 6/8/7/8 secunde și controlul **+5 secunde**.
- Butoane și personaje adaptate pentru mobil (390 px), tabletă (768 px), laptop (1440 px), tablă Samsung (1920×1080).
- A doua variantă care repeta povestea rămâne eliminată.

## Limitare tehnică importantă

Animațiile din poveste sunt de tip **2,5D**: mișcare cinematografică subtilă a cadrelor, tranziții și reacții vizuale. Nu reprezintă încă un film 3D cu personaje rigate, expresii faciale animate cadru-cu-cadru și sincronizare labială. Mai multe decoruri sunt ilustrații 3D generate, nu scene 3D geometrice interactive. Unele ilustrații de poveste sunt interpretări ale personajului, nu un model 3D unic rigat.

## Actualizare în repository-ul GitHub existent

Repository: `https://github.com/alinapalcu1-ship-it/maricica`

1. Folosește fișierul `Maricica_Update_Puzzle_Memory_3D.zip`.
2. Dezarhivează-l pe calculator.
3. Deschide pagina `https://github.com/alinapalcu1-ship-it/maricica/upload/main`.
4. Trage **conținutul** folderului extras: `index.html`, `v4.css`, `v4.js`, `README.md` și directorul `assets/cinema4/`.
5. Alege *Commit changes*. Fișierele vechi (`audio/`, `script.js`, `cinema.js`, `cinema.css`, `style.css` și alte imagini) trebuie **păstrate**.
6. GitHub Pages folosește deja `main / (root)`. După publicare, reîncarcă fără cache cu `Ctrl+F5` pe PC.

Pagina site-ului: `https://alinapalcu1-ship-it.github.io/maricica/`.

## Verificări automate efectuate

- Încărcare fără erori JavaScript în pagină la 390×844, 768×1024, 1440×900 și 1920×1080.
- Puzzle: toate cele 4 piese se pot plasa, apare felicitarea.
- Memory: 4 cartonașe și întoarcere de cartonaș.
- Ecrane de poveste: dormitor, baie, grădiniță.
- Nu s-au reînregistrat fișierele audio și nu s-au consumat credite ElevenLabs.

**Nu este verificat pe o tablă Samsung fizică.** Verifică pe dispozitiv sunetul, atingerea și scalarea la rezoluția folosită de tablă.

## Securitate și pedagogie

Fără conturi, fără reclame și fără colectarea datelor despre copii. Sursă audio: fișierele furnizate de utilizatoare. Narațiunea și ilustrațiile sunt folosite pentru activități educaționale; înainte de distribuire în afara unității, revizuiește drepturile de utilizare ale conținutului audio și ale adaptării.
