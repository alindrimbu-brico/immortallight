# Actualizarea site-ului — secțiunea Ediția Învățătorului

Se înlocuiesc **patru fișiere** în repo-ul `alindrimbu-brico/immortallight`. Restul rămâne neatins.

| Fișier | Ce e |
|---|---|
| `index.html` | **înlocuiește** varianta veche |
| `sitemap.xml` | **înlocuiește** (data s-a actualizat, ca Google să reindexeze) |
| `cover-teachers.png` | **nou** — coperta ediției engleze |
| `cover-teachers-ro.png` | **nou** — coperta ediției române |

## Pașii, pe GitHub

1. Deschide `https://github.com/alindrimbu-brico/immortallight`
2. **Add file → Upload files**
3. Trage toate patru fișierele din acest folder în zona de încărcare.
   GitHub le suprascrie pe cele două existente și le adaugă pe cele două noi.
4. Jos, la **Commit changes**, scrie în căsuța de sus:
   ```
   Secțiunea Ediția Învățătorului + linkurile Etsy
   ```
5. **Commit changes**.

Publicarea durează 1–2 minute. Verifică apoi la `https://immortallight.app/` — secțiunea nouă e între „Șapte piloni" și „Cartea", iar în meniul de sus a apărut **Pildele / The parables**.

## Ce s-a schimbat, ca să știi

- **Secțiune nouă, „Ediția Învățătorului"**, cu coperta, cele 55 de pilde, trei exemple de pilde cu izvoarele lor, și **două butoane care duc direct la listările Etsy** — engleza și româna.
- **Coperta se schimbă cu limba.** Pe EN arată coperta engleză, pe RO cea română. La fel și textul alternativ al imaginii.
- **Meniul de sus** are o intrare nouă: *The parables / Pildele*.
- **Butonul din hero**, „Get the book / Ia cartea", duce acum la secțiunea nouă — adică la singurul produs care chiar se poate cumpăra.
- **Secțiunea veche „Cartea"** se numește acum *Cartea întâi* și spune sincer că formatele ei sunt în pregătire, în loc să lase impresia că sunt de vânzare.
- **Datele structurate (JSON-LD)** conțin acum ambele ediții ale Ediției Învățătorului, cu preț, monedă, disponibilitate și adresa listării. Google poate afișa prețul direct în rezultate.
- **Descrierea paginii** pentru motoarele de căutare menționează pildele și izvoarele lor.

## Ce NU s-a atins

`LINKS` din `index.html` a rămas gol pentru paperback, Kindle, PDF-ul cărții întâi, printuri și Google Play. Cardurile lor arată în continuare „În curând", ceea ce e corect — produsele alea nu există încă. Când apar printurile pe Etsy, se completează `LINKS.prints` și cardul devine link.

## Verificat înainte de livrare

Pagina a fost deschisă într-un browser real, la 1280 px și la 390 px (telefon), în ambele limbi:
- fără depășire pe orizontală pe telefon (0 px);
- ambele coperți se încarcă;
- comutatorul de limbă schimbă corect textul, coperta și textul alternativ;
- JSON-LD parsează curat, cu patru ediții și două oferte;
- nicio cerere de fișier eșuată.
