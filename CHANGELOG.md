# Changelog

Alle nennenswerten Änderungen an HTTP-Atlas. Die Einträge beschreiben, was das Projekt
danach kann bzw. was sich für den Nutzer ändert – kein Commit-Protokoll.

**Regel:** Jeder Commit bekommt seinen Eintrag, im selben Commit. Neues kommt oben unter
„Unveröffentlicht“ dazu; beim Release wird daraus ein Abschnitt mit Versionsnummer und Datum.

Kategorien: **Neu** (neue Funktionen), **Verbessert** (bestehendes Verhalten), **Behoben**
(Fehler), **Intern** (Struktur, Tooling, nicht sichtbar).

## Unveröffentlicht

### Neu
- Erste Version: 16 Einträge in 5 Kapiteln (Anatomie einer Anfrage, Caching, Cookies & Speicher, CORS, Verbindung & Tempo),
  auf Deutsch und Englisch, mit Suche, hellem und dunklem Design, breiter Ansicht und
  App-Symbol.
- Simulationen: Jeder Regler ändert Anfrage und Antwort sofort; ein Urteil sagt, was der Browser daraus macht (cachen, blockieren, mitschicken …).
- Wasserfall: DNS, TCP, TLS, Warten und Download als Balken – wie im Network-Tab der DevTools.
- Echte Browser-APIs: Cookies setzen und löschen, den `storage`-Event zwischen Tabs sehen, Resource Timing einer echten Anfrage auslesen.
