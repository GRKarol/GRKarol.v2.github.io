# GRKarol.v2.github.io — Grankers Team

Statyczna witryna marki **Grankers Team**, hostowana na GitHub Pages.  
Projekt nie używa frameworka — czysty HTML5, CSS3, Vanilla JS.

---

## Struktura plików

```
/
├── index.html                     ← Strona główna (landing page, PUBLIC)
├── story.html                     ← Historia marki (PUBLIC)
│
├── shop.html                      ← Sklep internetowy (WIP, noindex)
│
├── work.html                      ← Prace w realizacji (noindex)
├── Dokładne plany.html            ← Wewnętrzne plany produktu (noindex)
├── progressio-covers-complete-1.html  ← Galeria okładek (noindex)
│
├── robots.txt                     ← SEO: tylko index.html i story.html publiczne
├── sitemap.xml                    ← Mapa witryny (2 publiczne strony)
├── site.webmanifest               ← PWA manifest
│
├── grankers-lion.png / .svg       ← Logo
├── grankers-team.jpg              ← Zdjęcie zespołu
└── favicon-*.png / .ico / .svg   ← Ikony (16–512px)
```

### Zasady widoczności

| Plik | SEO | Opis |
|------|-----|------|
| `index.html` | `index, follow` | Landing page — pre-order Progressio Journal |
| `story.html` | `index, follow` | Historia Grankers Team |
| `shop.html` | `noindex` | Sklep internetowy — w trakcie budowy |
| `work.html` | `noindex` | Behind-the-scenes, prace w toku |
| `Dokładne plany.html` | `noindex` | Plany wewnętrzne |
| `progressio-covers-complete-1.html` | `noindex` | Galeria okładek |

---

## Technologia

- **Frontend:** HTML5 + CSS3 + Vanilla JS (bez bundlera, bez frameworka)
- **Backend:** Firebase Firestore (lista oczekujących) + EmailJS (maile)
- **Hosting:** GitHub Pages
- **Czcionki:** Google Fonts CDN — Cinzel, Cormorant, Tenor Sans, Jost

## Design tokens

Ciemny luksusowy motyw. Zmienne CSS zdefiniowane w `:root` każdego pliku HTML:

| Token | Wartość | Rola |
|-------|---------|------|
| `--ink` | `#07060a` | Tło główne |
| `--gold` | `#c9a84c` | Akcent |
| `--parch` | `#ede0c4` | Tekst główny |
| `--serif` | Cormorant | Nagłówki |
| `--cinzel` | Cinzel | Etykiety / caps |
| `--ui` | Jost | Interfejs |

---

## Nawigacja

```
index.html ──→ story.html
           ──→ work.html
           ──→ shop.html (docelowo)
```

Routing oparty na plikach (brak SPA / JS routera).

---

## Aktualny status projektu

- [x] Landing page (`index.html`) — gotowy, publiczny
- [x] Strona historii (`story.html`) — gotowa, publiczna
- [ ] Sklep (`shop.html`) — **w planowaniu / budowie**
