# BT Tracker — Osobni zdravstveni dnevnik

> **Live app:** [borisobris.github.io/tezina](https://borisobris.github.io/tezina/)

Progresivna web aplikacija (PWA) za praćenje tjelesne težine, krvnog tlaka i tjelesnih mjera.  
Radi potpuno offline — podaci se čuvaju isključivo lokalno u pregledniku (localStorage).

---

## Značajke

- **Težina** — unos i grafički prikaz kroz vrijeme, trendline, BMI
- **Krvni tlak** — sistola / dijastola / puls, grafički prikaz
- **Tjelesne mjere** — struk, bokovi, prsa i ostalo
- **Aktivnosti** — unos i praćenje fizičke aktivnosti
- **Statistike** — tjedni pregled, napredak, min/max/prosjek
- **Backup / restore** — izvoz i uvoz podataka u JSON
- **Dark / light mode** — automatski prema sustavu
- **PWA** — instalabilna na Android, iOS, desktop; radi offline

---

## Instalacija (lokalno)

```bash
git clone https://github.com/BorisOrbis/tezina.git
cd tezina
# Posluži s bilo kojim HTTP serverom, npr:
npx serve .
# ili
python3 -m http.server 8080
```

Otvori `http://localhost:8080` u pregledniku.

---

## Struktura repozitorija

```
tezina/
├── index.html      # Cijela aplikacija (single-file PWA)
├── sw.js           # Service Worker za offline podršku
├── icon-192.png    # PWA ikona 192×192
├── icon-512.png    # PWA ikona 512×512
└── README.md
```

---

## GitHub Pages deploy

Repozitorij je konfiguriran za automatski deploy putem **GitHub Pages**.  
Svaki push na `main` granu odmah je dostupan na live URL-u.

**Postavke:** `Settings → Pages → Source: Deploy from branch → main / (root)`

---

## Privatnost

Svi podaci ostaju isključivo na uređaju korisnika.  
Nema servera, nema slanja podataka, nema analitike.

---

## Licenca

MIT — slobodno koristi, modificiraj, dijeli.
