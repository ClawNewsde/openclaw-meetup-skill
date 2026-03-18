[README.md](https://github.com/user-attachments/files/26096513/README.md)
# 🦞 claw://Meetup

Dein Radar für OpenClaw-Meetups und relevante AI-/Agent-Community-Events.

**claw://Meetup** hilft OpenClaw-Nutzern dabei, passende Events in ihrer Nähe zu finden, die besten Optionen zu priorisieren und auf Wunsch share-ready Texte oder Reminder-Flows vorzubereiten — ohne unnötigen Token-Verbrauch und ohne so zu tun, als gäbe es mehr Automatisierung als tatsächlich vorhanden ist.

## Funktionen

| Funktion | Beschreibung |
|---|---|
| 🦞 OpenClaw-first Discovery | Sucht zuerst nach OpenClaw-nahen Community-Events |
| 🔍 Eventsuche | Findet lokale Meetups, Hackathons und AI-/Agent-Events |
| 🎯 Shortlist & Best Pick | Sortiert und priorisiert die besten Treffer statt nur Listen auszukippen |
| 💬 Share Text | Erzeugt kurze, teilbare Event-Texte |
| 🔔 Reminder-Hilfe | Unterstützt bei Reminder-Setups mit sauberer Bestätigung |

## Installation

```bash
clawhub install meetup
```

Danach eine neue OpenClaw-Session starten.

## Typische Nutzung

Sag zum Agenten zum Beispiel:

| Anfrage | Was passiert |
|---|---|
| „Events near me“ | Sucht passende Events in deiner Nähe |
| „Find OpenClaw events in Berlin“ | Sucht gezielt nach OpenClaw-Events in Berlin |
| „Search AI agent meetups within 100 km“ | Sucht breiter nach AI-/Agent-Events |
| „Show me the best option“ | Empfiehlt den stärksten Treffer |
| „Share this event“ | Erstellt einen share-ready Text |
| „Remind me about this event“ | Startet einen Reminder-Flow |

## Wie der Skill arbeitet

`meetup` arbeitet in kleinen, token-effizienten Suchwellen:

1. **OpenClaw-first** — zuerst offizielle oder naheliegende OpenClaw-Quellen
2. **Breitere AI-/Agent-Suche** — wenn der Nutzer mehr will oder die erste Suche zu dünn ist
3. **Fallback-Websuche** — nur wenn nötig

Danach filtert der Skill hart:

- nur zukünftige Events
- nur sinnvolle lokale oder thematisch relevante Treffer
- keine doppelten oder schwachen Listings
- keine erfundenen Angaben zu Teilnehmerzahlen, Preisen oder Veranstaltern

## Skill-Struktur

```text
meetup/
├── SKILL.md
├── references/
│   ├── templates.md
│   ├── sources.md
│   ├── ranking.md
│   └── state-and-reminders.md
├── README.md
├── LICENSE
└── .gitignore
```

## Voraussetzungen

- Plattform: OpenClaw-Umgebungen mit Webzugriff
- Sprache: Mehrsprachig, Antwort in der Sprache des Nutzers
- Optimal mit: Persistentem Memory und Scheduler/Cron für echte Reminder
- Funktioniert auch ohne zusätzliche Persistenz: dann vor allem auf Abruf

## Release

### v1.0.0

- Initial public release of `meetup`
- Added OpenClaw-first event discovery workflow
- Added shortlist and best-pick ranking logic
- Added share-ready and reminder-oriented output templates
- Added source strategy, ranking, and state/reminder references
- Polished user-facing branding as **claw://Meetup**
- Packaged and validated for Skill Hub release

## Links

- 🌐 ClawHub: https://clawhub.ai/ClawNewsde/meetup
- 🌐 OpenClaw: https://openclaw.ai
- 🌐 ClawNews.de: https://clawnews.de
- 💬 Discord: https://discord.com/invite/qhfgMkjcaT
- 📧 Kontakt: mailto:skill@clawnews.de

## Lizenz

MIT License.
