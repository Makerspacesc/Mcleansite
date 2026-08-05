# Makerspace — Werkzeuge kurz & klar (Minimal-Version)

Eine bewusst **minimalistische** Ein-Seiten-Website für den Makerspace am
Peter-Wust-Gymnasium Wittlich. Sie zeigt nur das Nötigste: **welche Werkzeuge es
gibt, wofür man sie einsetzt und was zu beachten ist** – als ruhige
Scroll-Erzählung mit dezenten Effekten.

Abgeleitet vom ausführlichen [Werkzeug-Portal](https://github.com/edtechhackers-agents/makerspace-werkzeug-portal),
hier aber radikal reduziert: kein Menü, keine Suche, keine Filter – nur Inhalt.

Zwei Dateien, beide eigenständig – keine Build-Tools, keine Abhängigkeiten, kein Server:

- **`index.html`** – die minimalistische Übersichtsseite (kompaktes Karten-Raster,
  Scroll-Effekte) mit Button **„Zur Geräte-Bibliothek"**.
- **`bibliothek.html`** – die vollständige Geräte-Bibliothek im Stil des großen
  Portals: Karten-Raster mit **Suche**, **Kategoriefiltern** und **Detailansicht**
  (Technische Daten, Anwendung, Sicherheit, Kurzanleitung, Pflege, Prüfpunkte).
  Jede Detailansicht hat einen **Drucken-Button**, der nur die Infos des
  gewählten Werkzeugs sauber als Merkblatt ausgibt.

Beide Seiten sind **responsiv** (Handy, Tablet, Desktop).

## ✨ Effekte

- **Scroll-Fortschrittsbalken** am oberen Rand
- **Scroll-Reveal**: Inhalte fliegen gestaffelt ein, sobald sie sichtbar werden
- **Parallax** auf den Werkzeug-Icons (bewegen sich sanft beim Scrollen)
- **Hero-Titel** mit zeilenweiser Einblendung
- Weicher, mitlaufender Farbschimmer im Hintergrund
- Hell-/Dunkelmodus automatisch nach Systemeinstellung
- Alle Animationen respektieren `prefers-reduced-motion`

## 🧩 Inhalte pflegen

Alle Inhalte liegen als Daten oben im `<script>`-Block der `index.html`:

- **Werkzeuge** im Array `tools` – je Objekt: `icon`, `cat`, `title`, `use`,
  `spec`, `watch` (Liste der Warn-/Beachten-Punkte).
- **Allgemeine Regeln** im Array `rules`.
- **Impressum** im Objekt `IMPRESSUM`.

Verfügbare Icons (`icon`): `laser`, `printer`, `cnc`, `solder`, `hand`,
`measure`, `saw`, `drill`.

## 🚀 Nutzung

```bash
open index.html          # macOS  (Linux: xdg-open · Windows: start)
```

## 🔒 Datenschutz & Recht

Keine Datenerhebung, keine Cookies, nichts wird aus dem Netz geladen.
Alle Icons sind selbst erstellte Inline-SVGs; keine Fotos, keine fremden Assets.

## 📄 Lizenz

MIT – siehe [LICENSE](LICENSE).

---

Ein Projekt des Makerspace am Peter-Wust-Gymnasium Wittlich.
