# eskuvoi-video

Egyoldalas GitHub Pages oldal a Laura &amp; Viktor esküvői filmhez.

- **Domain:** `video.lauraesviktor.hu` (lásd `CNAME`)
- **Videó:** Google Drive-ban tárolva, a `/preview` végponton beágyazva
  (a Drive saját lejátszója — léptetés, hangerő, minőség, teljes képernyő).
- **Tartalék:** „Megnyitás a Drive-ban" gomb, Androidon `intent://` URL-lel,
  hogy a Drive alkalmazás nyíljon meg.

A videó cseréjéhez a fájl ID-t kell frissíteni az `index.html`-ben
(az `iframe` `src`-jében, a tartalék linkben és a `fileId` változóban).

A Drive-fájl megosztása maradjon „bárki, akinek megvan a link" — különben
a beágyazott lejátszó bejelentkezést kér.
