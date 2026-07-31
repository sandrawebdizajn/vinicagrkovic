# Vinica Grković — prezentacioni sajt

Statični sajt (jedan HTML fajl + folder sa slikama). Nema build koraka i nema zavisnosti.

## Struktura

    index.html      cela stranica (HTML + CSS + JS)
    images/         sve fotografije, logo i hero video
    robots.txt
    sitemap.xml
    .nojekyll       (potrebno za GitHub Pages)

## Lokalno pokretanje

Otvorite `index.html` u pregledaču, ili:

    python3 -m http.server 8000

## Objava na GitHub Pages

1. Napravite repozitorijum i prebacite sadržaj ovog foldera u koren (root).
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Sajt će biti dostupan na `https://<korisnik>.github.io/<repo>/`.

Ako sajt ide na svoj domen, dodajte `CNAME` fajl sa domenom i ispravite `canonical`,
`og:*` i `url` u JSON-LD u `index.html`.

## Šta treba dopuniti pre objave

- `[DOPUNITI AUTENTIČNOM PORODIČNOM PRIČOM, GODINAMA I FOTOGRAFIJAMA]` — sekcija Naša priča
- `[USLOVI ZA VEĆE PORUDŽBINE - POTVRDITI]`, `[PODRUČJE I USLOVI DOSTAVE - POTVRDITI]`,
  `[VRSTE I CENE POKLON-PAKOVANJA - POTVRDITI]`, `[USLOVI POSETE I DEGUSTACIJE - POTVRDITI]` — FAQ
- Recenzije su označene kao `PRIMER` — zamenite proverenim Google/Facebook recenzijama
- Radno vreme nije prikazano jer nije potvrđeno; kad se potvrdi, dodajte i
  `openingHoursSpecification` u JSON-LD
- Linkovi „Politika privatnosti" i „Politika kolačića" vode na `#`

## Kontakt podaci u kodu

Telefon `+381642619360`, email `vinicagrkovic@gmail.com`,
adresa `Ratka Pavlovića 124, Donja Vrežina, Niš`.
Ako se menjaju, promenite ih i u JSON-LD bloku na kraju `index.html`.
