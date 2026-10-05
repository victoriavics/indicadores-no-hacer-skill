# Skill «Indicadores No Hacer»

Un asistente para inteligencia artificial (Claude o ChatGPT) que ayuda a convertir recomendaciones **«No Hacer»** en indicadores de calidad asistencial medibles, y a revisarlos y evaluarlos.

Acompaña al libro sobre indicadores «No Hacer» (en preparación) y está pensado para equipos de calidad asistencial que trabajan con recomendaciones «No Hacer», MAPAC, Choosing Wisely, Compromiso por la Calidad y marcos equivalentes.

## Cómo instalarlo

**Instrucciones paso a paso, con capturas: https://victoriavics.github.io/indicadores-no-hacer-skill/**

### Claude (claude.ai o la app de escritorio)

1. Abre **Customize → Plugins**, pulsa **+ Add** y elige **Add marketplace → Add from a repository**.
2. En **URL** escribe `victoriavics/indicadores-no-hacer-skill`, elige la opción **Use "victoriavics/indicadores-no-hacer-skill"** y pulsa **Sync**.
3. Cuando aparezca **Indicadores no hacer**, pulsa **Add**. Si sale un aviso sobre *Auto-sync*, ciérralo.

### ChatGPT (chatgpt.com o la app de escritorio)

1. Descarga **[indicadores-no-hacer.zip](https://github.com/victoriavics/indicadores-no-hacer-skill/releases/latest/download/indicadores-no-hacer.zip)**.
2. En ChatGPT, abre **Customize → Skills**, pulsa **Add** y elige **Upload from your computer**.
3. Selecciona el zip.

### Codex

```bash
codex plugin marketplace add victoriavics/indicadores-no-hacer-skill
codex plugin add indicadores-no-hacer@indicadores-no-hacer
```

### Claude Code

Dentro de Claude Code:

```
/plugin marketplace add victoriavics/indicadores-no-hacer-skill
/plugin install indicadores-no-hacer@indicadores-no-hacer
```

### npx skills (varios agentes a la vez)

```bash
npx skills add victoriavics/indicadores-no-hacer-skill -g
```

## Cómo usarlo

No hay que aprender comandos. Basta con escribir lo que se necesita, por ejemplo:

- Pegar una recomendación «No Hacer» y pedir que la analice.
- «Hazme la ficha técnica de este indicador.»
- Aportar los datos de un pilotaje y pedir la concordancia entre evaluadores.

Si no se concreta qué análisis se quiere, el skill muestra el menú y pregunta por dónde empezar.

## Qué hace

Ofrece ocho análisis **independientes**. Se pueden usar sueltos o encadenados; ninguno exige haber hecho los anteriores.

| # | Análisis | Qué necesita |
|---|---|---|
| 1 | Afinar la recomendación (precisión de actuación, población y excepciones) | La recomendación |
| 2 | Detectar errores de clasificación (falsos positivos y negativos, zonas grises) | La recomendación |
| 3 | Decidir cómo medirla (adecuación AA, sobreutilización SU u otro enfoque) | La recomendación |
| 4 | Construir los indicadores | Una o varias recomendaciones |
| 5 | Revisar los indicadores con bibliografía | La tabla de indicadores |
| 6 | Ficha técnica de un indicador (vía directa) | Recomendación + enfoque |
| 7 | Ficha de evaluación para un panel de expertos | La ficha técnica |
| 8 | Analizar un pilotaje (factibilidad y fiabilidad interobservador) | Ficha técnica + datos |

Cuando se encadenan dos análisis, el skill se detiene y recuerda qué quedó validado y qué quedó pendiente, para que los errores de un paso no se arrastren al siguiente.

Los resultados pueden entregarse en **Word, Excel o PDF**.

## Principio de funcionamiento

La regla que gobierna todo el skill: **no inventar**. Ni criterios clínicos, ni indicaciones, ni excepciones, ni poblaciones, ni umbrales, ni ventanas temporales, ni sistemas de información, ni referencias o DOI. Lo que no se deduce del texto aportado o de una aclaración validada por el usuario se señala como información pendiente.

El criterio de calidad es la reproducibilidad: que dos evaluadores independientes, con los mismos datos y las mismas reglas, clasifiquen igual el mismo caso.

## Para quien quiera ver por dentro

```
skills/indicadores-no-hacer/   El skill
  SKILL.md                     Punto de entrada: elección del análisis, tono y encadenado
  router.md                    Los ocho análisis, para qué sirven y qué necesitan
  core.md                      Definiciones (AA, SU, excepción, exclusión, aclaración) y reglas transversales
  state.md                     Qué se conserva entre análisis y cómo se plantea la pausa al encadenar
  modules/                     Un archivo por análisis
  output/                      Reglas de formato (Word, Excel, PDF)
.claude-plugin/                Plugin y marketplace para Claude Code
.codex-plugin/                 Plugin para Codex / ChatGPT
.agents/plugins/               Marketplace para Codex / ChatGPT
```

Cada versión publicada está en [Releases](https://github.com/victoriavics/indicadores-no-hacer-skill/releases), y los cambios en [CHANGELOG.md](CHANGELOG.md).
