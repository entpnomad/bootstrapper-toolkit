🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md)

# Bootstrapper Toolkit

Un toolkit de [Claude Code skills](https://docs.anthropic.com/en/docs/claude-code/skills) qui aide les fondateurs à évaluer des idées business avec la rigueur du bootstrapper. Conçu pour les fondateurs qui s'autofinancent avec le revenu client, pas le capital-risque.

Alimenté par une bibliothèque curatée de livres business — stratégie, positionnement, pricing, croissance, unit economics, et plus encore. Les skills distillent les enseignements de dizaines de livres en analyses structurées, pour que tu aies des frameworks éprouvés au combat sans avoir à lire toute l'étagère toi-même.

## Skills Complémentaires

Une fois l'idée validée, utilise ceux-ci pour construire et optimiser :
- [flag-theory](https://github.com/entpnomad/flag-theory) — Optimise ta structure internationale (incorporation, résidence fiscale, banque) pour le business que tu construis
- [tone-of-voice](https://github.com/entpnomad/tone-of-voice) — Définis la voix de ta marque avant d'écrire des landing pages et du contenu
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimise le contenu pour les moteurs de réponse LLM et les agents IA
- [seo-rank](https://github.com/entpnomad/seo-rank) — Audit et optimisation SEO aux standards 2026

## Ce que ça fait

Tape `/analyze-idea` dans Claude Code et décris une idée business. Le toolkit lance 10 agents de recherche spécialisés en parallèle, note l'idée selon un framework quantitatif, et synthétise un verdict stratégique — le tout ancré dans des données de marché réelles via la recherche web.

Chaque dimension peut aussi tourner de façon autonome :

| Skill | Ce qu'il fait |
|-------|---------------|
| `/analyze-idea` | Analyse complète orchestrée — lance toutes les dimensions, note, synthétise |
| `/venture-sensei` | Mentorat stratégique brutal et critique de l'idée |
| `/bootstrap-oracle` | Notation structurée avec unit economics et filtres de bon sens |
| `/competitor-analysis` | Intelligence concurrentielle sur 16 dimensions |
| `/market-size` | TAM/SAM/SOM bottom-up avec validation de la demande |
| `/problem-analysis` | Sévérité de la douleur, disposition à payer, clarté du buyer persona |
| `/solution-analysis` | Adéquation produit, différenciation, menace de substitution par l'IA |
| `/gtm-strategy` | Beachhead, canaux, économie de distribution, 100 premiers clients |
| `/moat-analysis` | Défensibilité, coûts de changement, lock-in par investissement utilisateur |
| `/timing-analysis` | Fenêtre de marché, points d'inflexion, vulnérabilité des incumbents |
| `/business-model` | Architecture de revenus, pricing, structure de marges, design de l'offre |
| `/financial-projections` | Cash flow, break-even, paliers de revenus, stress tests |
| `/founder-fit` | Clarté du domaine, accès à la distribution, tempo d'exécution, diagnostic des 8 habitudes |

## Philosophie

**Le revenu est le seul tour de financement.**

- Pas de mentalité VC, pas de pensée exit-first, pas de théâtre de valorisation
- Construis des choses pour lesquelles les gens paient, puis capitalise sur des décennies
- Le meilleur moment pour vendre un bon business, c'est jamais

Le code est bon marché — les outils IA de développement permettent à un fondateur solo de livrer ce qui nécessitait avant une équipe financée. Le goulot d'étranglement est passé de « peut-on le construire ? » à la **clarté** (sais-tu ce qui vaut la peine d'être construit ?) et la **distribution** (peux-tu atteindre les acheteurs ?). Chaque skill de ce toolkit pondère en conséquence.

## Installation

1. Clone ce repo
2. Ouvre le répertoire du projet dans Claude Code
3. Lance n'importe quel skill : `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, etc.

Les skills sont locaux au projet (`.claude/skills/`), pas globaux. Ils s'activent automatiquement quand Claude Code ouvre ce répertoire.

## Structure du Projet

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Conventions du projet et architecture des skills
├── .claude/skills/                    # Tous les skills (locaux au projet)
│   ├── _shared/                       # Philosophie et principes partagés
│   ├── analyze-idea/                  # Orchestrateur — lance toutes les dimensions
│   ├── venture-sensei/                # Mentor — critique stratégique
│   ├── bootstrap-oracle/              # Mentor — notation structurée
│   ├── competitor-analysis/           # Skill de dimension
│   ├── market-size/                   # Skill de dimension
│   ├── problem-analysis/              # Skill de dimension
│   ├── solution-analysis/             # Skill de dimension
│   ├── gtm-strategy/                  # Skill de dimension
│   ├── moat-analysis/                 # Skill de dimension
│   ├── timing-analysis/               # Skill de dimension
│   ├── business-model/                # Skill de dimension
│   ├── financial-projections/         # Skill de dimension
│   └── founder-fit/                   # Skill de dimension
└── references/                        # Bibliothèque curatée de livres business (PDFs) + INDEX.md
```

## Pourquoi ça existe

Avant, je faisais tout ça à la main.

Pendant des années, j'ai évalué des idées business de la manière lente — lire des livres, monter des tableurs, chercher des données de marché sur Google avec 20 onglets ouverts, faire de l'analyse concurrentielle à la main. Chaque nouvelle idée, c'était des jours de recherche avant d'avoir assez de signal pour décider si ça valait le coup de construire.

Mes frameworks se sont affinés à chaque business. MetricSpot m'a appris ce que signifie vraiment penser distribution-first. RevenueHunt m'a appris que l'idée compte moins que le canal. Une décennie à tout essayer — une agence de marketing digital, des produits ratés, des idées qui ont brûlé des mois pour rien — m'a appris quelles questions comptent vraiment. Certaines choses ont marché. Mais le SaaS avec distribution freemium, c'est ce qui a scalé.

Mais le processus restait lent, manuel et enfermé dans ma tête.

Puis l'IA est devenue assez bonne pour changer l'équation. Pas « résume-moi cet article » bonne — assez bonne pour lancer 10 agents de recherche en parallèle, récupérer des données de marché réelles, noter une idée contre un framework quantitatif, et synthétiser un verdict meilleur que ce que produisent la plupart des consultants. Environ 30 minutes, pas des jours — et ça creuse en profondeur.

Alors j'ai pris chaque framework que j'avais construit en une décennie — les grilles de notation, les dimensions concurrentielles, les contrôles de bon sens en unit economics, les diagnostics de founder-fit — et je les ai transformés en skills Claude Code. La bibliothèque de référence, c'est plus de 30 livres business que j'ai réellement lus et appliqués. Les poids de notation reflètent ce que j'ai appris en construisant deux businesses rentables à partir de zéro.

Ce toolkit, c'est mon processus de décision, automatisé. Il est opinioné parce que je le suis.

## Crédits

Créé par [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), cofondateur de [RevenueHunt](https://www.revenuehunt.com/) — un SaaS bootstrappé à 7 chiffres construit sans capital-risque. Le skill Oracle scoring est inspiré d'un framework de [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), membre de [Dynamite Circle](https://dynamitecircle.com/).

Lis la version pour humains sur [Founders Hub](https://founders.do).
