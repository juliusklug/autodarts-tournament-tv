# AutoDarts Tournament TV

Öffentliche Zuschauer-/TV-Ansicht für den AutoDarts Tournament Companion.

## Geplante Live-Adresse

https://autodarts.tv.hiddenhits.de

## Technik

- Statische Webseite über GitHub Pages
- Turnierdaten und Realtime über Supabase
- Zuschauer haben ausschließlich Lesezugriff
- Schreibzugriff bleibt beim Tournament Companion
- AutoDarts-Zugangsdaten werden nicht an die TV-Seite übertragen

## GitHub Pages

Repository öffentlich anlegen, danach:

1. `index.html`, `.nojekyll` und `CNAME` in `main` hochladen.
2. Settings → Pages
3. Source: **Deploy from a branch**
4. Branch: **main**, Ordner: **/(root)**
5. Speichern

Der `CNAME`-Eintrag ist bereits auf `autodarts.tv.hiddenhits.de` vorbereitet.

## Dynadot

Nach Aktivierung von GitHub Pages wird bei Dynadot ein CNAME für die Subdomain benötigt:

- Host/Subdomain: `autodarts.tv`
- Typ: `CNAME`
- Ziel: `juliusklug.github.io`

Danach kann GitHub das HTTPS-Zertifikat für `autodarts.tv.hiddenhits.de` bereitstellen.
