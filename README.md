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

- [x] Elérhetőségek: telefon +36 30 462 5292, e-mail konyveles@gondamonika.hu (2026-08-24)
- [x] Vélemények: Tudatos Diák / T-DIGITAL / T-Cloud Kft. (2026-08-24)
- [x] Árak: konkrét összegek helyett ajánlat-alapú csomagok (2026-08-24)
- [x] `adatvedelem.html` kitöltve a hivatalos EV-adatokkal (2026-08-24)
- [x] Blog: 3 SEO-cikk a `blog/` alatt, sitemap bővítve (2026-08-24)
- [x] DNS-rekordok felvíve a Rackhostnál (2026-08-24)
- [ ] Portréfotó a Rólam szekcióba (`gondamonika-portre.jpg`)
- [ ] Levelezés: `konyveles@` → átirányítás közvetlenül Mónika Gmailjébe (MX + SPF/DKIM/DMARC a dns24 zónában) — Mónikával közösen állítjuk be
- [x] DNS-delegálás rendben, domain újramentve a Pages-en → cert-kiadás folyamatban (2026-08-27)
- [ ] Enforce HTTPS pipa bekapcsolása a GitHub Pages-en, amint a cert kiadódott
- [ ] Google Search Console felvétel + sitemap beküldés; Google Cégprofil (Business Profile)
- [ ] Vélemény-szövegek jóváhagyatása a nevesített személyekkel (Yilmaz A., Szabó L., Galgóczi A.)

## E-mail (konyveles@gondamonika.hu) — beállítás

A weboldal a GitHub-on van, a levelezéshez KÜLÖN e-mail szolgáltatás kell:

1. Rackhost admin → e-mail képes szolgáltatás a domainhez (webtárhely vagy önálló
   e-mail tárhely csomag), azon belül postafiók: `konyveles@gondamonika.hu`.
2. A DNS-zónába (ugyanott, ahol az A-rekordok vannak) a Rackhost által megadott
   **MX rekord(ok)** + **SPF TXT** rekord felvétele. (Rackhost tárhelynél ezeket
   gyakran automatikusan felajánlja/beszúrja a szolgáltatás aktiválásakor.)
3. **Választott megoldás:** e-mail *átirányítás* közvetlenül Mónika saját Gmail-címére,
   és a Gmailben „Küldés másként" beállítása a konyveles@ címmel.
