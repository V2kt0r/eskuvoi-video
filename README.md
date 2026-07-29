# eskuvoi-video

Átirányító oldal a Laura &amp; Viktor esküvői filmhez, a `jegyesfotozas`
repo mintájára.

- **Domain:** `video.lauraesviktor.hu` (lásd `CNAME`)
- **Cél:** a Google Drive-ban tárolt videó (`/view`), ahol a Drive saját
  lejátszója/alkalmazása játssza le — natív kezelőszervekkel.

## Miért átirányítás, és nem beágyazott lejátszó?

Volt egy beágyazott változat (Drive `/preview` iframe-ben), de a Drive
lejátszójának kezelőszervei egy másik domainen futnak, így CSS-ből nem
formázhatók, és telefonon aránytalanul nagyra/félrecsúszva jelentek meg.
A beágyazás a git history-ban megvan, ha valaha kellene.

Saját `<video>` lejátszó sem járható út: a film 4K, 6 perc 26 másodperc,
**2,42 GB**, adaptív minőség nélkül — mobilnetről használhatatlan lenne.
A Drive ezzel szemben kisebb felbontásra kódolja át.

A videó cseréjéhez a fájl ID-t kell frissíteni az `index.html`-ben (2 helyen).
A Drive-fájl megosztása maradjon „bárki, akinek megvan a link".
