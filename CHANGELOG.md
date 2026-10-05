# Registro de cambios

Formato basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/).

## [1.1.1] — 2026-10-06

### Cambiado
- El repositorio pasa a ser instalable como plugin en Claude Code y en Codex / ChatGPT de escritorio. La skill se mueve a `skills/indicadores-no-hacer/`.
- Se retira `empaquetar.sh`: el zip para claude.ai se publica en Releases.

### Sin cambios
- Contenido de la skill.

## [1.1.0] — 2026-08-25

### Añadido
- Menú de entrada: si no se concreta qué se quiere hacer, el skill presenta los ocho análisis en lenguaje natural y espera la elección, en lugar de ejecutar por su cuenta.
- Entrada mínima explícita en cada análisis, para poder usar cualquiera de forma aislada sin haber hecho los anteriores.
- Aviso de arrastre al encadenar análisis: resumen breve de lo validado y lo pendiente, y una pregunta antes de continuar.
- Salida en **Excel** (`output/excel_rules.md`): hojas de trabajo reales con filtros, una fila por registro, vaciado de puntuaciones del panel de expertos y cálculos de factibilidad y Kappa vinculados a los datos del pilotaje.
- Salida en **PDF** (`output/pdf_rules.md`), con paginación cuidada y refuerzo textual de las marcas para impresión en blanco y negro.
- `output/formats.md`: elección de formato según el entregable y reglas comunes a los tres.

### Cambiado
- Tono general: se retiran los códigos internos (M1–M8) y el lenguaje de procedimiento de cara al usuario.
- Los checkpoints rígidos (VALIDADO / MODIFICAR / PENDIENTE / BLOQUEANTE) se mantienen como lógica interna, pero se expresan como conversación.
- `router.md` pasa a ser una tabla de elección con la entrada mínima de cada análisis.
- `state.md` se reescribe alrededor de qué se conserva entre análisis y por qué importa la pausa.

### Sin cambios
- Todo el contenido metodológico: definiciones de AA y SU, reglas de no invención, estructura de salida de cada análisis y reglas de formato Word.

## [1.0.0] — 2026-08-21

- Primera versión: ocho módulos, núcleo metodológico, estado y checkpoints, y reglas de salida Word.
