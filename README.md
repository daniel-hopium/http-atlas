# HTTP-Atlas – HTTP & Browser zum Anfassen

Requests und Responses, Statuscodes, Caching, Cookies, CORS und Verbindungen zum Durchspielen: Regler setzen, die simulierte Anfrage und Antwort ablesen, dazu echte Demos mit `document.cookie`, `localStorage` und der Resource Timing API deines Browsers.

16 Einträge in 5 Kapiteln, auf Deutsch und Englisch.

Online: https://daniel-hopium.github.io/http-atlas/

## Starten

`index.html` im Browser öffnen, per Doppelklick. Kein Build, kein Server, keine
Abhängigkeiten. Internet braucht es nur für die Google-Schriften.

## Inhalt

| Kapitel | Einträge |
|---|---|
| Anatomie einer Anfrage | Aufbau einer URL, Methoden, Statuscodes, Redirects, Content Negotiation |
| Caching | Cache-Control, ETag und 304, Cache-Busting |
| Cookies & Speicher | Cookie-Attribute, Echte Cookies setzen, Wo der Browser speichert |
| CORS | CORS-Simulator, Origin oder Site? |
| Verbindung & Tempo | Vor dem ersten Byte, HTTP/1.1 gegen HTTP/2, Echt gemessen |

Jeder Eintrag hat eine eigene Adresse (`#kapitel/eintrag`), die meisten eine Stolperfalle
oder einen Merksatz und Links zu MDN oder der passenden Doku. Der Überblick hat eine
durchsuchbare Tabelle aller Einträge.

## So funktioniert es

- **Simulationen:** Jeder Regler ändert Anfrage und Antwort sofort; ein Urteil sagt, was der Browser daraus macht (cachen, blockieren, mitschicken …).
- **Wasserfall:** DNS, TCP, TLS, Warten und Download als Balken – wie im Network-Tab der DevTools.
- **Echte Browser-APIs:** Cookies setzen und löschen, den `storage`-Event zwischen Tabs sehen, Resource Timing einer echten Anfrage auslesen.

## Bedienung

- **Sprache:** Der Link oben rechts („English“ / „Deutsch“) wechselt die Sprache. Sie steht
  als `?lang=en` in der Adresse (teilbar), wird im `localStorage` gemerkt und folgt sonst der
  Browsersprache.
- `Strg+K` (Mac: `Cmd+K`) springt in die Suche der Seitenleiste.
- Hell und dunkel folgen der Systemeinstellung; der Sonne/Mond-Knopf überschreibt sie.
- Ab 1280px Breite schaltet der Breite-Knopf die breite Ansicht ein; dort lässt sich die
  Lektion am Griff rechts schmaler oder breiter ziehen.

## Aufbau

Alles steckt in einer Datei, `index.html`:

- **Hülle:** Kopfleiste, Seitenleiste mit Suche, Router, Sprache, Theme und Breite – dieselbe
  wie in den Schwester-Apps.
- **`CATS` und `ENTRIES`:** die Kapitel und ein Objekt pro Eintrag mit Text (`desc`, `tip`,
  `rule`, `links`) und einer Demo-Art (`kind`): `run` (echter Code mit Konsole), `trace`
  (Schritt-für-Schritt-Zustände), `sim` (Regler → Ergebnis) oder `custom` (eigene Demo mit
  `html()` und `init()`, die eine Aufräumfunktion zurückgibt).
- **Zweisprachig:** `tx('Deutsch','English')` steht direkt neben jedem Text.
- **Icons:** `tools/make_icons.py` erzeugt `favicon.svg`, `favicon.ico` und
  `apple-touch-icon.png` aus einer Geometrie (braucht Pillow).

## Schwester-Apps

[UI-Atlas](https://daniel-hopium.github.io/ui-atlas/), [CSS-Atlas](https://daniel-hopium.github.io/css-atlas/), [HTML-Atlas](https://daniel-hopium.github.io/html-atlas/), [ARIA-Kompass](https://daniel-hopium.github.io/aria-compass/), [Angular-Patterns](https://daniel-hopium.github.io/angular-patterns/), [Rechte-Kompass](https://daniel-hopium.github.io/access-compass/), [JS-Laufzeit](https://daniel-hopium.github.io/js-runtime/), [Sicherheits-Labor](https://daniel-hopium.github.io/security-lab/), [Performance-Atlas](https://daniel-hopium.github.io/perf-atlas/), [Regex-Werkstatt](https://daniel-hopium.github.io/regex-lab/), [Algorithmen-Visualizer](https://daniel-hopium.github.io/algo-visualizer/).
