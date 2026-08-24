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

- [ ] Placeholder elérhetőségek cseréje (telefon, e-mail, cím) az `index.html`-ben
- [ ] Portréfotó a Rólam szekcióba
- [ ] Statisztikák (év tapasztalat, ügyfélszám) valós adatokra igazítása
