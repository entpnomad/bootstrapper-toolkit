🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

# Bootstrapper Toolkit

Um toolkit de [Claude Code skills](https://docs.anthropic.com/en/docs/claude-code/skills) que ajuda fundadores a avaliar ideias de negócio com o rigor de quem se autofinancia. Feito para fundadores que crescem com receita de clientes, não com capital de risco.

Alimentado por uma biblioteca curada de livros de negócio — estratégia, posicionamento, pricing, crescimento, unit economics e mais. Os skills destilam insights de dezenas de livros em análises estruturadas, para que tenhas frameworks testados em batalha sem precisar ler a estante inteira.

## Skills Complementares

Depois de validar a ideia, usa estes para construir e otimizar:
- [flag-theory](https://github.com/entpnomad/flag-theory) — Otimiza a tua estrutura internacional (incorporação, residência fiscal, banca) para o negócio que estás a construir
- [tone-of-voice](https://github.com/entpnomad/tone-of-voice) — Define a voz da tua marca antes de escrever landing pages e conteúdo
- [ai-rank](https://github.com/entpnomad/ai-rank) — Otimiza conteúdo para motores de resposta LLM e agentes de IA
- [seo-rank](https://github.com/entpnomad/seo-rank) — Auditoria e otimização SEO ao padrão de 2026

## O que faz

Escreve `/analyze-idea` no Claude Code e descreve uma ideia de negócio. O toolkit lança 10 agentes de investigação especializados em paralelo, pontua a ideia com um framework quantitativo e sintetiza um veredicto estratégico — tudo baseado em dados reais de mercado via pesquisa web.

Cada dimensão também funciona de forma independente:

| Skill | O que faz |
|-------|-----------|
| `/analyze-idea` | Análise completa orquestrada — executa todas as dimensões, pontua, sintetiza |
| `/venture-sensei` | Mentoria estratégica brutal e crítica da ideia |
| `/bootstrap-oracle` | Pontuação estruturada com unit economics e filtros de sanidade |
| `/competitor-analysis` | Inteligência competitiva em 16 dimensões |
| `/market-size` | TAM/SAM/SOM bottom-up com validação de procura |
| `/problem-analysis` | Severidade da dor, disposição para pagar, clareza do buyer persona |
| `/solution-analysis` | Adequação do produto, diferenciação, ameaça de substituição por IA |
| `/gtm-strategy` | Beachhead, canais, economia de distribuição, primeiros 100 clientes |
| `/moat-analysis` | Defensabilidade, custos de mudança, lock-in por investimento do utilizador |
| `/timing-analysis` | Janela de mercado, pontos de inflexão, vulnerabilidade de incumbentes |
| `/business-model` | Arquitetura de receitas, pricing, estrutura de margens, design da oferta |
| `/financial-projections` | Cash flow, break-even, degraus de receita, stress tests |
| `/founder-fit` | Clareza de domínio, acesso a distribuição, ritmo de execução, diagnóstico de 8 hábitos |

## Filosofia

**A receita é a única ronda de financiamento.**

- Nada de mentalidade VC, nada de pensar em exit primeiro, nada de teatro de avaliação
- Constrói coisas pelas quais as pessoas pagam, depois capitaliza durante décadas
- O melhor momento para vender um bom negócio é nunca

O código é barato — as ferramentas de IA para programar permitem que um fundador solo lance o que antes exigia uma equipa financiada. O bottleneck passou de "conseguimos construir isto?" para **clareza** (sabes o que vale a pena construir?) e **distribuição** (consegues chegar aos compradores?). Cada skill deste toolkit pondera em conformidade.

## Instalação

1. Clona este repo
2. Abre o diretório do projeto no Claude Code
3. Executa qualquer skill: `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, etc.

Os skills são locais ao projeto (`.claude/skills/`), não globais. Ativam-se automaticamente quando o Claude Code abre este diretório.

## Estrutura do Projeto

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Convenções do projeto e arquitetura de skills
├── .claude/skills/                    # Todos os skills (locais ao projeto)
│   ├── _shared/                       # Filosofia e princípios partilhados
│   ├── analyze-idea/                  # Orquestrador — executa todas as dimensões
│   ├── venture-sensei/                # Mentor — crítica estratégica
│   ├── bootstrap-oracle/              # Mentor — pontuação estruturada
│   ├── competitor-analysis/           # Skill de dimensão
│   ├── market-size/                   # Skill de dimensão
│   ├── problem-analysis/              # Skill de dimensão
│   ├── solution-analysis/             # Skill de dimensão
│   ├── gtm-strategy/                  # Skill de dimensão
│   ├── moat-analysis/                 # Skill de dimensão
│   ├── timing-analysis/               # Skill de dimensão
│   ├── business-model/                # Skill de dimensão
│   ├── financial-projections/         # Skill de dimensão
│   └── founder-fit/                   # Skill de dimensão
└── references/                        # Biblioteca curada de livros de negócio (PDFs) + INDEX.md
```

## Porque é que isto existe

Eu costumava fazer tudo isto manualmente.

Durante anos, avaliei ideias de negócio da forma lenta — a ler livros, a montar folhas de cálculo, a pesquisar dados de mercado no Google com 20 separadores abertos, a fazer análise competitiva à mão. Cada nova ideia significava dias de investigação antes de ter sinal suficiente para decidir se valia a pena construir.

Os meus frameworks ficaram mais afinados com cada negócio. O MetricSpot ensinou-me o que realmente significa pensar distribution-first. O RevenueHunt ensinou-me que a ideia importa menos do que o canal. Uma década a tentar de tudo — uma agência de marketing digital, produtos falhados, ideias que queimaram meses sem chegar a lado nenhum — ensinou-me quais perguntas realmente importam. Algumas coisas funcionaram. Mas SaaS com distribuição freemium é o que escalou.

Mas o processo continuava lento, manual e fechado na minha cabeça.

Depois a IA ficou boa o suficiente para mudar a equação. Não "resume-me este artigo" boa — boa o suficiente para executar 10 agentes de investigação em paralelo, obter dados reais de mercado, pontuar uma ideia contra um framework quantitativo e sintetizar um veredicto melhor do que o que a maioria dos consultores produz. Cerca de 30 minutos, não dias — e vai a fundo.

Então peguei em cada framework que tinha construído ao longo de uma década — as grelhas de pontuação, as dimensões competitivas, os controlos de sanidade de unit economics, os diagnósticos de founder-fit — e transformei-os em skills de Claude Code. A biblioteca de referência são mais de 30 livros de negócio que realmente li e apliquei. Os pesos de pontuação refletem o que aprendi ao construir dois negócios rentáveis a partir do zero.

Este toolkit é o meu processo de tomada de decisão, automatizado. É opinativo porque eu sou.

## Créditos

Criado por [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), cofundador da [RevenueHunt](https://www.revenuehunt.com/) — um SaaS bootstrapped de 7 dígitos construído sem capital de risco. O skill Oracle scoring foi inspirado num framework de [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), membro do [Dynamite Circle](https://dynamitecircle.com/).

Lê a versão para humanos no [Founders Hub](https://founders.do).
