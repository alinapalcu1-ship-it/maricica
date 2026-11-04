# Maricica învață să fie curată — versiunea CINEMA 3D

**Poveste animată + joc educațional cu voce în limba română, pentru grupa mică (3 ani).** Adaptare pedagogică după „Maricica”, de Luiza Vlădescu.

## Ce am schimbat

- Am eliminat opțiunea **„Povestește și joacă-te”**, care relua narațiunea.
- Meniul principal oferă două trasee clare: **Ascultă povestea** și **Ne jucăm cu Maricica!**.
- Am păstrat **exact același model vizual** pentru Maricica. Au fost construite două variante, cu murdărie ușoară și îngrijită, fără schimbarea fizionomiei.
- Am introdus o colegă de grădiniță 3D și un ursuleț de pluș 3D.
- Am refăcut elementele principale de igienă în stil 3D și fundalurile tuturor celor șase momente.
- Am adăugat mișcare 2,5D (personaje construite din straturi ale unor imagini 3D): gesturi cu brațele, balans, reacții la dialog, reacții ale ursulețului, obiecte animate, particule și tranziții lente. **Nu este un film 3D cu animație facială completă**.
- Am păstrat **55 MP3 pentru poveste** și **19 MP3 pentru partea interactivă** din ElevenLabs.
- Jocul oprește redarea după întrebări și așteaptă alegerea copilului. Exercițiile de mișcare au pauze după terminarea audio: 6, 8, 7, 8 secunde, plus butoane pentru **+5 secunde** și **Gata, mai departe**.
- Fără reclame, cont, monitorizare sau clasamente.

## Instalare în repository-ul existent `maricica`

Dacă ai deja jocul vechi pe GitHub, **nu reîncărca audio și fișierele vechi**. Folosește pachetul mic de actualizare:

1. Dezarhivează `Maricica_Update_3D_GitHub.zip` pe calculator.
2. Deschide repository-ul `https://github.com/alinapalcu1-ship-it/maricica` și alege `Add file` → `Upload files`.
3. Trage **conținutul** pachetului: `index.html`, `cinema.css`, `cinema.js`, `README.md` și directorul `assets/cinema`.
4. Acceptă înlocuirea `index.html`/`README.md` dacă apare solicitarea și apasă `Commit changes`.
5. GitHub Pages va construi din nou site-ul automat. Actualizează pagina cu `Ctrl+F5` pentru a evita versiunea salvată în cache.

Linkul rămâne `https://alinapalcu1-ship-it.github.io/maricica/`.

## Structură tehnică

- `index.html` — pagina principală, adaugă modulul cinematic
- `style.css` + `script.js` — funcționalitățile originale, inclusiv audio și pauzele
- `cinema.css` + `cinema.js` — noul design, distribuția personajelor, gesturi 2,5D și meniul simplificat
- `assets/cinema/` — Maricica curată/neîngrijită, brațe separate, ursuleț, colega de grădiniță, decoruri, obiecte 3D
- `audio/01.mp3` … `55.mp3` — poveste
- `audio/interactive/01.mp3` … `19.mp3` — jocul interactiv

## Testare înainte de activitatea cu copiii

Testele automate de navigare și afișare au fost rulate la 390×844, 1024×768 și 1440×900. Este necesară verificarea **pe tabla Samsung reală** pentru audio, dimensiuni, latență și calitatea animațiilor.

Parcurge cele 6 momente și verifică dacă murdăria se vede la grădiniță, dar dispare după îngrijire; verifică și colega, ursulețul și cele 3 întrebări. Apoi lasă să se încheie cele 4 pauze de mișcare; pentru copii, poți folosi butonul `+5 secunde`.

**Notă drepturi:** verifică dreptul de publicare a adaptării poveștii și condițiile de utilizare/publicare a înregistrărilor generate în ElevenLabs, în funcție de planul folosit. Ilustrațiile 3D folosite sunt materiale vizuale realizate pentru acest proiect.
