🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md)

# Bootstrapper Toolkit

Un toolkit de [Claude Code skills](https://docs.anthropic.com/en/docs/claude-code/skills) que ayuda a fundadores a evaluar ideas de negocio con el rigor de quien se autofinancia. Pensado para fundadores que crecen con ingresos de clientes, no con capital de riesgo.

Funciona con una biblioteca curada de libros de negocio — estrategia, posicionamiento, pricing, crecimiento, unit economics y más. Los skills destilan las ideas de decenas de libros en análisis estructurados, para que tengas frameworks probados en batalla sin tener que leerte toda la estantería.

## Skills Complementarios

Una vez validada la idea, usa estos para construir y optimizar:
- [flag-theory](https://github.com/entpnomad/flag-theory) — Optimiza tu estructura internacional (incorporación, residencia fiscal, banca) para el negocio que estás construyendo
- [tone-of-voice](https://github.com/entpnomad/tone-of-voice) — Define la voz de tu marca antes de escribir landing pages y contenido
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimiza contenido para motores de respuesta LLM y agentes de IA
- [seo-rank](https://github.com/entpnomad/seo-rank) — Auditoría y optimización SEO al estándar de 2026

## Qué hace

Escribe `/analyze-idea` en Claude Code y describe una idea de negocio. El toolkit lanza 10 agentes de investigación especializados en paralelo, puntúa la idea con un framework cuantitativo y sintetiza un veredicto estratégico — todo basado en datos reales de mercado vía búsqueda web.

Cada dimensión también funciona de forma independiente:

| Skill | Qué hace |
|-------|----------|
| `/analyze-idea` | Análisis completo orquestado — ejecuta todas las dimensiones, puntúa, sintetiza |
| `/venture-sensei` | Mentoría estratégica brutal y crítica de la idea |
| `/bootstrap-oracle` | Puntuación estructurada con unit economics y filtros de cordura |
| `/competitor-analysis` | Inteligencia competitiva en 16 dimensiones |
| `/market-size` | TAM/SAM/SOM bottom-up con validación de demanda |
| `/problem-analysis` | Severidad del dolor, disposición a pagar, claridad del buyer persona |
| `/solution-analysis` | Encaje del producto, diferenciación, amenaza de sustitución por IA |
| `/gtm-strategy` | Beachhead, canales, economía de distribución, primeros 100 clientes |
| `/moat-analysis` | Defensibilidad, costes de cambio, lock-in por inversión del usuario |
| `/timing-analysis` | Ventana de mercado, puntos de inflexión, vulnerabilidad de incumbentes |
| `/business-model` | Arquitectura de ingresos, pricing, estructura de márgenes, diseño de oferta |
| `/financial-projections` | Flujo de caja, break-even, escalones de ingresos, stress tests |
| `/founder-fit` | Claridad de dominio, acceso a distribución, tempo de ejecución, diagnóstico de 8 hábitos |

## Filosofía

**Los ingresos son la única ronda de financiación.**

- Nada de mentalidad VC, nada de pensar en exit primero, nada de teatro de valoración
- Construye cosas por las que la gente pague, luego capitaliza durante décadas
- El mejor momento para vender un buen negocio es nunca

El código es barato — las herramientas de IA para programar hacen que un fundador solo pueda lanzar lo que antes requería un equipo financiado. El cuello de botella ha pasado de "¿podemos construirlo?" a **claridad** (¿sabes qué vale la pena construir?) y **distribución** (¿puedes llegar a los compradores?). Cada skill de este toolkit pondera en consecuencia.

## Instalación

1. Clona este repo
2. Abre el directorio del proyecto en Claude Code
3. Ejecuta cualquier skill: `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, etc.

Los skills son locales al proyecto (`.claude/skills/`), no globales. Se activan automáticamente cuando Claude Code abre este directorio.

## Estructura del Proyecto

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Convenciones del proyecto y arquitectura de skills
├── .claude/skills/                    # Todos los skills (locales al proyecto)
│   ├── _shared/                       # Filosofía y principios compartidos
│   ├── analyze-idea/                  # Orquestador — ejecuta todas las dimensiones
│   ├── venture-sensei/                # Mentor — crítica estratégica
│   ├── bootstrap-oracle/              # Mentor — puntuación estructurada
│   ├── competitor-analysis/           # Skill de dimensión
│   ├── market-size/                   # Skill de dimensión
│   ├── problem-analysis/              # Skill de dimensión
│   ├── solution-analysis/             # Skill de dimensión
│   ├── gtm-strategy/                  # Skill de dimensión
│   ├── moat-analysis/                 # Skill de dimensión
│   ├── timing-analysis/               # Skill de dimensión
│   ├── business-model/                # Skill de dimensión
│   ├── financial-projections/         # Skill de dimensión
│   └── founder-fit/                   # Skill de dimensión
└── references/                        # Biblioteca curada de libros de negocio (PDFs) + INDEX.md
```

## Por qué existe esto

Antes hacía todo esto a mano.

Durante años, evalué ideas de negocio de la forma lenta — leyendo libros, armando hojas de cálculo, buscando datos de mercado en Google con 20 pestañas abiertas, haciendo análisis competitivo a mano. Cada nueva idea significaba días de investigación antes de tener suficiente señal para decidir si valía la pena construirla.

Mis frameworks se afinaron con cada negocio. MetricSpot me enseñó lo que realmente significa pensar primero en distribución. RevenueHunt me enseñó que la idea importa menos que el canal. Una década probándolo todo — una agencia de marketing digital, productos fallidos, ideas que quemaron meses sin llegar a nada — me enseñó qué preguntas realmente importan. Algunas cosas funcionaron. Pero SaaS con distribución freemium es lo que escaló.

Pero el proceso seguía siendo lento, manual y encerrado en mi cabeza.

Entonces la IA se volvió suficientemente buena para cambiar la ecuación. No "resúmeme este artículo" buena — suficientemente buena para ejecutar 10 agentes de investigación en paralelo, obtener datos reales de mercado, puntuar una idea contra un framework cuantitativo y sintetizar un veredicto mejor que lo que producen la mayoría de consultores. Unos 30 minutos, no días — y va a fondo.

Así que tomé cada framework que había construido en una década — las rúbricas de puntuación, las dimensiones competitivas, los controles de cordura de unit economics, los diagnósticos de founder-fit — y los convertí en skills de Claude Code. La biblioteca de referencia son más de 30 libros de negocio que realmente leí y apliqué. Los pesos de puntuación reflejan lo que aprendí construyendo dos negocios rentables desde cero.

Este toolkit es mi proceso de toma de decisiones, automatizado. Es opinado porque yo lo soy.

## Créditos

Creado por [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), cofundador de [RevenueHunt](https://www.revenuehunt.com/) — un SaaS bootstrapped de 7 cifras construido sin capital de riesgo. El skill Oracle scoring se inspiró en un framework de [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), miembro de [Dynamite Circle](https://dynamitecircle.com/).

Lee la versión para humanos en [Founders Hub](https://founders.do).
