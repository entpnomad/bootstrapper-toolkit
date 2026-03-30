🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

# Bootstrapper Toolkit

Ein [Claude Code Skills](https://docs.anthropic.com/en/docs/claude-code/skills)-Toolkit, das Gründern hilft, Geschäftsideen mit Bootstrapper-Rigorosität zu bewerten. Gebaut für Gründer, die sich aus Kundeneinnahmen finanzieren, nicht aus Risikokapital.

Angetrieben von einer kuratierten Referenzbibliothek aus Business-Büchern — Strategie, Positionierung, Pricing, Wachstum, Unit Economics und mehr. Die Skills destillieren Erkenntnisse aus Dutzenden von Büchern in strukturierte Analysen, damit du kampferprobte Frameworks bekommst, ohne das ganze Regal selbst lesen zu müssen.

## Begleitende Skills

Sobald die Idee validiert ist, nutze diese zum Bauen und Optimieren:
- [flag-theory](https://github.com/entpnomad/flag-theory) — Optimiere dein internationales Setup (Firmengründung, Steuerresidenz, Banking) für das Business, das du aufbaust
- [tone-of-voice](https://github.com/entpnomad/tone-of-voice) — Definiere deine Markenstimme, bevor du Landing Pages und Content schreibst
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimiere Content für LLM-Antwortmaschinen und KI-Agenten
- [seo-rank](https://github.com/entpnomad/seo-rank) — SEO-Audit und -Optimierung nach 2026-Standards

## Was es macht

Tippe `/analyze-idea` in Claude Code ein und beschreibe eine Geschäftsidee. Das Toolkit startet 10 spezialisierte Research-Agenten parallel, bewertet die Idee anhand eines quantitativen Frameworks und synthetisiert ein strategisches Urteil — alles gestützt auf reale Marktdaten via Web-Recherche.

Jede Dimension kann auch einzeln laufen:

| Skill | Was er macht |
|-------|-------------|
| `/analyze-idea` | Vollständige orchestrierte Analyse — führt alle Dimensionen aus, bewertet, synthetisiert |
| `/venture-sensei` | Brutales strategisches Mentoring und Ideenkritik |
| `/bootstrap-oracle` | Strukturierte Bewertung mit Unit Economics und Plausibilitätsprüfungen |
| `/competitor-analysis` | Wettbewerbs-Intelligence über 16 Dimensionen |
| `/market-size` | Bottom-up TAM/SAM/SOM mit Nachfragevalidierung |
| `/problem-analysis` | Schmerzintensität, Zahlungsbereitschaft, Klarheit der Buyer Persona |
| `/solution-analysis` | Produkteignung, Differenzierung, KI-Substitutionsbedrohung |
| `/gtm-strategy` | Beachhead, Kanäle, Distributionsökonomie, erste 100 Kunden |
| `/moat-analysis` | Verteidigungsfähigkeit, Wechselkosten, Lock-in durch Nutzerinvestition |
| `/timing-analysis` | Marktfenster, Wendepunkte, Verwundbarkeit der Incumbents |
| `/business-model` | Umsatzarchitektur, Pricing, Margenstruktur, Angebotsdesign |
| `/financial-projections` | Cash Flow, Break-even, Umsatzstufen, Stresstests |
| `/founder-fit` | Domänenwissen, Distributionszugang, Ausführungstempo, 8-Gewohnheiten-Diagnose |

## Philosophie

**Umsatz ist die einzige Finanzierungsrunde.**

- Keine VC-Mentalität, kein Exit-first-Denken, kein Bewertungstheater
- Baue Dinge, für die Leute bezahlen, dann lass sie über Jahrzehnte wachsen
- Der beste Zeitpunkt, ein gutes Business zu verkaufen, ist nie

Code ist billig — KI-Coding-Tools ermöglichen es einem Solo-Gründer, zu liefern, wofür früher ein finanziertes Team nötig war. Der Engpass hat sich verschoben von „können wir es bauen?" zu **Klarheit** (weißt du, was es wert ist, gebaut zu werden?) und **Distribution** (erreichst du die Käufer?). Jeder Skill in diesem Toolkit gewichtet entsprechend.

## Setup

1. Klone dieses Repo
2. Öffne das Projektverzeichnis in Claude Code
3. Starte einen beliebigen Skill: `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, etc.

Skills sind projektlokal (`.claude/skills/`), nicht global. Sie aktivieren sich automatisch, wenn Claude Code dieses Verzeichnis öffnet.

## Projektstruktur

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Projektkonventionen und Skill-Architektur
├── .claude/skills/                    # Alle Skills (projektlokal)
│   ├── _shared/                       # Geteilte Philosophie und Prinzipien
│   ├── analyze-idea/                  # Orchestrator — führt alle Dimensionen aus
│   ├── venture-sensei/                # Mentor — strategische Kritik
│   ├── bootstrap-oracle/              # Mentor — strukturierte Bewertung
│   ├── competitor-analysis/           # Dimensions-Skill
│   ├── market-size/                   # Dimensions-Skill
│   ├── problem-analysis/              # Dimensions-Skill
│   ├── solution-analysis/             # Dimensions-Skill
│   ├── gtm-strategy/                  # Dimensions-Skill
│   ├── moat-analysis/                 # Dimensions-Skill
│   ├── timing-analysis/               # Dimensions-Skill
│   ├── business-model/                # Dimensions-Skill
│   ├── financial-projections/         # Dimensions-Skill
│   └── founder-fit/                   # Dimensions-Skill
└── references/                        # Kuratierte Business-Buchbibliothek (PDFs) + INDEX.md
```

## Warum es das gibt

Ich habe das alles früher manuell gemacht.

Jahrelang habe ich Geschäftsideen auf die langsame Art bewertet — Bücher lesen, Spreadsheets bauen, Marktdaten in 20 Browser-Tabs googeln, Wettbewerbsanalysen von Hand machen. Jede neue Idee bedeutete Tage an Recherche, bevor ich genug Signal hatte, um zu entscheiden, ob sie es wert war, gebaut zu werden.

Meine Frameworks wurden mit jedem Business schärfer. MetricSpot hat mir beigebracht, was Distribution-first-Denken wirklich bedeutet. RevenueHunt hat mir beigebracht, dass die Idee weniger zählt als der Kanal. Ein Jahrzehnt, in dem ich alles ausprobiert habe — eine Digitalagentur, gescheiterte Produkte, Ideen, die Monate verbrannt haben und nirgendwohin führten — hat mir beigebracht, welche Fragen wirklich zählen. Einiges hat funktioniert. Aber SaaS mit Freemium-Distribution ist das, was skaliert hat.

Aber der Prozess war immer noch langsam, manuell und in meinem Kopf eingesperrt.

Dann wurde KI gut genug, um die Gleichung zu verändern. Nicht „fass mir diesen Artikel zusammen" gut — gut genug, um 10 Research-Agenten parallel laufen zu lassen, echte Marktdaten zu ziehen, eine Idee gegen ein quantitatives Framework zu bewerten und ein Urteil zu synthetisieren, das besser ist als das, was die meisten Berater liefern. Etwa 30 Minuten, nicht Tage — und es geht in die Tiefe.

Also nahm ich jedes Framework, das ich über ein Jahrzehnt aufgebaut hatte — die Bewertungsraster, die Wettbewerbsdimensionen, die Unit-Economics-Plausibilitätsprüfungen, die Founder-Fit-Diagnosen — und verwandelte sie in Claude Code Skills. Die Referenzbibliothek umfasst über 30 Business-Bücher, die ich tatsächlich gelesen und angewandt habe. Die Bewertungsgewichte spiegeln wider, was ich beim Aufbau zweier profitabler Businesses von Null gelernt habe.

Dieses Toolkit ist mein Entscheidungsprozess, automatisiert. Es ist meinungsstark, weil ich es bin.

## Credits

Erstellt von [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), Mitgründer von [RevenueHunt](https://www.revenuehunt.com/) — ein 7-stelliges bootstrapped SaaS, aufgebaut ohne Risikokapital. Der Oracle-Scoring-Skill wurde inspiriert von einem Framework von [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), einem Mitglied des [Dynamite Circle](https://dynamitecircle.com/).

Lies die menschenfreundliche Version auf [Founders Hub](https://founders.do).
