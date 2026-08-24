# gondamonika.hu

Gonda Monika — könyvelés és bérszámfejtés landing oldal.

- **Stack:** statikus HTML (nincs build lépés), GitHub Pages
- **Domain:** gondamonika.hu (Rackhost DNS → GitHub Pages)
- **Élesítés:** push a `main`-re → Pages automatikusan frissül

## DNS (Rackhost DNS-zóna)

| Típus | Név | Érték |
|-------|-----|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | szaboleonardhenrik.github.io. |

A GitHub Pages beállításokban a custom domain: `gondamonika.hu` (a repo `CNAME`
fájlja tartalmazza), az „Enforce HTTPS" a tanúsítvány kiállítása után kapcsolható be.

## Teendők élesítés előtt

- [ ] Placeholder elérhetőségek cseréje (telefon, e-mail, cím) az `index.html`-ben + JSON-LD-ben
- [ ] Portréfotó a Rólam szekcióba (`gondamonika-portre.jpg`)
- [ ] Statisztikák (év tapasztalat, ügyfélszám) valós adatokra igazítása
- [ ] Árak szekció: minta-havidíjak valós díjakra cserélése (vagy árak elrejtése)
- [ ] Vélemények: minta-idézetek valós ügyfél-visszajelzésekre cserélése
- [ ] `adatvedelem.html` véglegesítése (adatkezelő adatai, adószám, nyilvántartási szám)
- [ ] `info@gondamonika.hu` postafiók létrehozása (Rackhost) + SPF/DKIM/MX rekordok
- [ ] DNS-rekordok felvitele a Rackhostnál (fenti táblázat), utána Enforce HTTPS a GitHub-on
- [ ] Google Search Console felvétel + sitemap beküldés; Google Cégprofil (Business Profile)
