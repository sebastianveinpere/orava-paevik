# Orava päevik

Isiklik PWA: kalorid, vesi, paastutaimer, nädala statistika, kalender, eesmärgid (nädal, kuu, aasta), visioonitahvel ja orav, keda saab silitada, toita ja magama panna.

## Failid

- `index.html`: kogu äpp (HTML, CSS ja JavaScript ühes failis)
- `manifest.webmanifest`: äpi nimi, värvid ja ikoonid avaekraani jaoks
- `sw.js`: service worker, tänu millele äpp töötab ka ilma võrguta
- `icon-*.png`, `apple-touch-icon.png`: äpi ikoonid

## Ülespanek GitHub Pagesi

1. Repo seadetes ava **Settings → Pages**.
2. Vali **Deploy from a branch**, haru `main` ja kaust `/ (root)`.
3. Paari minuti pärast on äpp aadressil `https://<kasutaja>.github.io/<repo>/`.

## iPhone'i avaekraanile

Ava aadress Safaris, vajuta jagamise nuppu ja vali **Add to Home Screen**.

## Andmed

Kõik andmed on ainult selles seadmes (localStorage, visioonitahvli pildid IndexedDB-s). Varukoopia saab kopeerida seadetest; pildid varukoopiasse ei lähe.

## Uuendamine

Kui muudad `index.html` faili, tõsta `sw.js` failis `VERSION` väärtust (nt `orav-v2`), et telefon uue versiooni alla laeks.
