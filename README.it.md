🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

# Bootstrapper Toolkit

Un toolkit di [Claude Code skills](https://docs.anthropic.com/en/docs/claude-code/skills) che aiuta i founder a valutare idee di business con il rigore di chi si autofinanzia. Pensato per founder che crescono con i ricavi dei clienti, non con il venture capital.

Alimentato da una libreria curata di libri di business — strategia, posizionamento, pricing, crescita, unit economics e altro. Gli skill distillano gli insegnamenti di decine di libri in analisi strutturate, così hai framework collaudati sul campo senza doverti leggere tutto lo scaffale.

## Skill Complementari

Una volta validata l'idea, usa questi per costruire e ottimizzare:
- [flag-theory](https://github.com/entpnomad/flag-theory) — Ottimizza la tua struttura internazionale (incorporazione, residenza fiscale, banca) per il business che stai costruendo
- [tone-of-voice](https://github.com/entpnomad/tone-of-voice) — Definisci la voce del tuo brand prima di scrivere landing page e contenuti
- [ai-rank](https://github.com/entpnomad/ai-rank) — Ottimizza i contenuti per i motori di risposta LLM e gli agenti IA
- [seo-rank](https://github.com/entpnomad/seo-rank) — Audit e ottimizzazione SEO agli standard 2026

## Cosa fa

Scrivi `/analyze-idea` in Claude Code e descrivi un'idea di business. Il toolkit lancia 10 agenti di ricerca specializzati in parallelo, valuta l'idea con un framework quantitativo e sintetizza un verdetto strategico — tutto basato su dati di mercato reali tramite ricerca web.

Ogni dimensione può anche funzionare in autonomia:

| Skill | Cosa fa |
|-------|---------|
| `/analyze-idea` | Analisi completa orchestrata — esegue tutte le dimensioni, valuta, sintetizza |
| `/venture-sensei` | Mentorship strategica brutale e critica dell'idea |
| `/bootstrap-oracle` | Valutazione strutturata con unit economics e filtri di buon senso |
| `/competitor-analysis` | Intelligence competitiva su 16 dimensioni |
| `/market-size` | TAM/SAM/SOM bottom-up con validazione della domanda |
| `/problem-analysis` | Severità del problema, disponibilità a pagare, chiarezza del buyer persona |
| `/solution-analysis` | Adeguatezza del prodotto, differenziazione, minaccia di sostituzione IA |
| `/gtm-strategy` | Beachhead, canali, economia di distribuzione, primi 100 clienti |
| `/moat-analysis` | Difendibilità, costi di cambio, lock-in da investimento dell'utente |
| `/timing-analysis` | Finestra di mercato, punti di inflessione, vulnerabilità degli incumbent |
| `/business-model` | Architettura dei ricavi, pricing, struttura dei margini, design dell'offerta |
| `/financial-projections` | Cash flow, break-even, gradini di ricavo, stress test |
| `/founder-fit` | Chiarezza del dominio, accesso alla distribuzione, tempo di esecuzione, diagnostica delle 8 abitudini |

## Filosofia

**Il fatturato è l'unico round di finanziamento.**

- Niente mentalità VC, niente pensiero exit-first, niente teatro della valutazione
- Costruisci cose per cui la gente paga, poi capitalizza per decenni
- Il momento migliore per vendere un buon business è mai

Il codice costa poco — gli strumenti IA per programmare permettono a un founder solo di lanciare quello che prima richiedeva un team finanziato. Il collo di bottiglia si è spostato da "possiamo costruirlo?" alla **chiarezza** (sai cosa vale la pena costruire?) e alla **distribuzione** (riesci a raggiungere i compratori?). Ogni skill di questo toolkit pesa di conseguenza.

## Installazione

1. Clona questo repo
2. Apri la directory del progetto in Claude Code
3. Lancia qualsiasi skill: `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, ecc.

Gli skill sono locali al progetto (`.claude/skills/`), non globali. Si attivano automaticamente quando Claude Code apre questa directory.

## Struttura del Progetto

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Convenzioni del progetto e architettura degli skill
├── .claude/skills/                    # Tutti gli skill (locali al progetto)
│   ├── _shared/                       # Filosofia e principi condivisi
│   ├── analyze-idea/                  # Orchestratore — esegue tutte le dimensioni
│   ├── venture-sensei/                # Mentor — critica strategica
│   ├── bootstrap-oracle/              # Mentor — valutazione strutturata
│   ├── competitor-analysis/           # Skill di dimensione
│   ├── market-size/                   # Skill di dimensione
│   ├── problem-analysis/              # Skill di dimensione
│   ├── solution-analysis/             # Skill di dimensione
│   ├── gtm-strategy/                  # Skill di dimensione
│   ├── moat-analysis/                 # Skill di dimensione
│   ├── timing-analysis/               # Skill di dimensione
│   ├── business-model/                # Skill di dimensione
│   ├── financial-projections/         # Skill di dimensione
│   └── founder-fit/                   # Skill di dimensione
└── references/                        # Libreria curata di libri di business (PDF) + INDEX.md
```

## Perché esiste

Prima facevo tutto questo a mano.

Per anni ho valutato idee di business nel modo lento — leggendo libri, costruendo fogli di calcolo, cercando dati di mercato su Google con 20 tab aperti, facendo analisi competitiva a mano. Ogni nuova idea significava giorni di ricerca prima di avere abbastanza segnale per decidere se valeva la pena costruirla.

I miei framework si sono affinati con ogni business. MetricSpot mi ha insegnato cosa significa davvero pensare distribution-first. RevenueHunt mi ha insegnato che l'idea conta meno del canale. Un decennio a provare di tutto — un'agenzia di digital marketing, prodotti falliti, idee che hanno bruciato mesi senza portare a nulla — mi ha insegnato quali domande contano davvero. Alcune cose hanno funzionato. Ma il SaaS con distribuzione freemium è quello che ha scalato.

Ma il processo restava lento, manuale e chiuso nella mia testa.

Poi l'IA è diventata abbastanza buona da cambiare l'equazione. Non "riassumimi questo articolo" buona — abbastanza buona da lanciare 10 agenti di ricerca in parallelo, recuperare dati di mercato reali, valutare un'idea contro un framework quantitativo e sintetizzare un verdetto migliore di quello che producono la maggior parte dei consulenti. Circa 30 minuti, non giorni — e va in profondità.

Così ho preso ogni framework che avevo costruito in un decennio — le griglie di valutazione, le dimensioni competitive, i controlli di buon senso sulle unit economics, le diagnostiche di founder-fit — e li ho trasformati in skill di Claude Code. La libreria di riferimento sono più di 30 libri di business che ho davvero letto e applicato. I pesi di valutazione riflettono quello che ho imparato costruendo due business profittevoli da zero.

Questo toolkit è il mio processo decisionale, automatizzato. È opinionato perché io lo sono.

## Crediti

Creato da [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), cofondatore di [RevenueHunt](https://www.revenuehunt.com/) — un SaaS bootstrapped da 7 cifre costruito senza venture capital. Lo skill Oracle scoring è ispirato a un framework di [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), membro di [Dynamite Circle](https://dynamitecircle.com/).

Leggi la versione per umani su [Founders Hub](https://founders.do).
