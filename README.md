# Stop Slop (Deutsch)

Eine Skill für das Entfernen von KI-Sprachmustern aus deutschen Texten.

## Was das ist

KI-Texte haben Muster. Vorhersehbare Phrasen, Strukturen, Rhythmen. Diese Skill bringt Claude (oder jedes andere LLM) dazu, sie zu erkennen und zu entfernen — auf Deutsch.

## Struktur

```
stop-slop-de/
├── SKILL.md              # Kernanweisungen
├── references/
│   ├── phrases.md        # Zu entfernende Phrasen
│   ├── structures.md     # Zu vermeidende Strukturmuster
│   └── examples.md       # Vorher/Nachher-Transformationen
├── README.md
├── CHANGELOG.md
└── LICENSE
```

## Schnellstart

**Claude Code:** Diesen Ordner als Skill hinzufügen.

**Claude Projects:** `SKILL.md` und die Referenzdateien in das Projektwissen hochladen.

**Benutzerdefinierte Anweisungen:** Kernregeln aus `SKILL.md` kopieren.

**API-Aufrufe:** `SKILL.md` in den System-Prompt einbinden. Referenzdateien werden bei Bedarf geladen.

## Was erkannt wird

**Verbotene Phrasen** — Ankündigungseinleitungen, Betonungskrücken, Geschäftsjargon, alle Adverbien, vage Aussagen, Meta-Kommentare. Siehe `references/phrases.md`.

**Strukturelle Klischees** — Binäre Gegensätze, negative Aufzählungen, dramatische Fragmentierung, rhetorische Aufbauten, falsche Handlungsträgerschaft, Erzähler-aus-der-Distanz-Stimme, Passiv. Siehe `references/structures.md`.

**Satzebene** — Keine W-Frage-Satzanfänge, keine Gedankenstriche, keine Stakkato-Fragmentierung, keine faulen Extreme, Aktiv erforderlich.

## Bewertung

Punkte von 1-10 in jeder Dimension:

| Dimension | Frage |
|-----------|-------|
| Direktheit | Aussagen oder Ankündigungen? |
| Rhythmus | Abwechslungsreich oder gleichförmig? |
| Vertrauen | Respektiert die Intelligenz des Lesers? |
| Authentizität | Klingt es menschlich? |
| Dichte | Gibt es Kürzbares? |

Unter 35/50: überarbeiten.

## Autor

Original: [Hardik Pandya](https://hvpandya.com)  
Deutsche Übersetzung und Anpassung

## Lizenz

MIT. Frei verwendbar, gerne teilen.
