# Changelog — Ifrits AutoBeater

Alle nennenswerten Änderungen. / All notable changes.
**[🇩🇪 Deutsch](#deutsch) · [🇬🇧 English](#english)**

<a name="deutsch"></a>
## 🇩🇪 Deutsch

### v4.2
- Zielabstand-Standard auf **1,0 s** — entspricht der Marker-Dichte echter Lighttoys-Shows (50–60/min).

| Zielabstand | Marker/min | Abdeckung echter Cuts |
|---|---|---|
| 0,5 s | ~85 | 48 % |
| 1,0 s (Standard) | ~54 | 32 % |
| 2,0 s | ~37 | 24 % |

### v4.1
- Drei abschaltbare Show-Filter steuern die Marker-Menge (Beat-Raster / nur Schläge mit hörbarem Einsatz / ruhige Passagen ausdünnen).
- Zielabstand wirkt als echter Mindestabstand — kleiner = mehr Abdeckung, größer = ruhigeres Bild.

### v4.0 — deutlich bessere Treffer
- Engine an echten Lighttoys-Shows kalibriert (3 Projekte, 3100 programmierte Elemente).
- Kernbefund: Programmierer schneiden **auf dem Beat** (69 % exakt), nicht an den lautesten Stellen.
- **Hochpräzise Tempo-Erkennung** (±0,01 BPM statt ±2 BPM) — der Grund, warum ein BPM-Raster früher „nicht mehr passte".
- Neuer **rasterbasierter Show-Modus**.
- Gemessen gegen echte Shows: Trefferquote **11 % → 59 %**, F1 **14 % → 37 %**.
- Modi neu sortiert und mit klaren Anwendungsfällen beschrieben.

### v3.4
- Show-Modus verfeinert: gleichmäßige Abdeckung ohne lange Leerbereiche, Median-Abstand ~3 s wie in echten Shows, Dichte folgt dem Energiekontrast.
- Begleitdatei füllt zusätzlich `sections`, `bpm` und `drop_ms`.

### v3.3
- Kurzer Workflow-Hinweis oben (Projekt erst im LtComposer bauen, Musik laden, speichern → dann Marker setzen).
- Breiteres, kompakteres Fenster; Modi 3-spaltig.
- Begleitdatei ist jetzt eine versteckte Experten-Option.

### v3.2
- Ausgabename jetzt `<Projekt>_IfritsAB-<Modus>.ltp`.
- Es wird **immer** eine neue .ltp mit den Markern erzeugt; die Originaldatei bleibt garantiert unverändert.
- Bestehende Ausgaben werden nie überschrieben (`_2`, `_3` …).

### v3.1
- Projektdatei jetzt **byte-genau** im LtComposer-Stil (Fließkomma-Schreibweise korrigiert).
- Fenster passt sich dem Bildschirm an, Scrollbalken bei Bedarf.
- Show-Modus ist Standard.

### v3.0
- Neuer **Show-Modus**: Struktur-Marker an Sektionsgrenzen plus Akzente, deren Dichte der Energie folgt (dicht im Drop, ruhig im Break, Zielabstand ~3 s).
- Optionale Begleitdatei `.IfritsBeats.json` mit Sektionen, Energie & Tempo.
- Projektdatei wird jetzt exakt im LtComposer-Stil geschrieben.

### v2.0
- Sprachen DE / EN / CZ (umschaltbar, wird gespeichert).
- Dynamisches Beat-Tracking, das Tempo-Änderungen im Lied folgt.
- Alle Einstellungen dauerhaft sichtbar mit Erklärungen.
- Fertige EXE für Windows.

<a name="english"></a>
## 🇬🇧 English

### v4.2
- Default target spacing is now **1.0 s** — matching the marker density of real Lighttoys shows (50–60/min).

| Target spacing | Markers/min | Coverage of real cuts |
|---|---|---|
| 0.5 s | ~85 | 48 % |
| 1.0 s (default) | ~54 | 32 % |
| 2.0 s | ~37 | 24 % |

### v4.1
- Three switchable Show filters control marker density (beat grid / only beats with an audible hit / thin out quiet passages).
- Target spacing now acts as a real minimum distance — smaller = more coverage, larger = a calmer picture.

### v4.0 — much better hit rate
- Engine calibrated against real Lighttoys shows (3 projects, 3100 programmed elements).
- Key finding: programmers cut **on the beat** (69 % exactly), not at the loudest moments.
- **High-precision tempo detection** (±0.01 BPM instead of ±2 BPM) — exactly why a BPM grid used to "drift off" over time.
- New **grid-based Show mode**.
- Measured against the real shows: recall **11 % → 59 %**, F1 **14 % → 37 %**.
- Modes reordered and described with clear use cases.

### v3.4
- Show mode refined: even coverage without long empty stretches, median spacing ~3 s like real shows, density follows the actual energy contrast.
- Companion file also fills `sections`, `bpm` and `drop_ms`.

### v3.3
- Short workflow hint at the top (build the project in LtComposer first, load music, save → then set markers).
- Wider, more compact window; modes in 3 columns.
- The companion file is now a hidden expert option.

### v3.2
- Output name is now `<project>_IfritsAB-<mode>.ltp`.
- A new .ltp with the markers is **always** created; the original file is guaranteed to stay unchanged.
- Existing outputs are never overwritten (`_2`, `_3` …).

### v3.1
- Project file now **byte-exact** in LtComposer style (float notation fixed).
- Window adapts to your screen, scrollbar when needed.
- Show mode is the default.

### v3.0
- New **Show mode**: structure markers at section boundaries plus accents whose density follows the energy (dense in the drop, calm in the break, target spacing ~3 s).
- Optional companion file `.IfritsBeats.json` with sections, energy & tempo.
- The project file is now written exactly in LtComposer style.

### v2.0
- Languages DE / EN / CZ (switchable, remembered).
- Dynamic beat tracking that follows tempo changes within a song.
- All settings permanently visible with explanations.
- Ready-to-run EXE for Windows.
