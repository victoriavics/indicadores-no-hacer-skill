# 2 · Detectar errores de clasificación

## Objetivo
Analizar si la recomendación permite discriminar correctamente entre cumplimiento e incumplimiento, prestando especial atención a las excepciones.

## Entrada mínima
La recomendación «No Hacer». Si ya hay aclaraciones validadas en la conversación, úsalas; si no las hay, este análisis se puede hacer igualmente y no exige haber revisado antes la precisión.

## Instrucciones
Valorar:
- **Falsos positivos**: casos clasificados como incumplimiento aunque la actuación estuviera justificada; identificar excepciones ausentes, incompletas o demasiado restrictivas que puedan provocarlos.
- **Falsos negativos**: casos clasificados como adecuados o excluidos cuando deberían considerarse incumplimientos; identificar excepciones demasiado amplias, ambiguas o fácilmente aplicables.
- **Capacidad de discriminación**: comprobar si los criterios permiten separar objetivamente cumplimiento e incumplimiento e identificar zonas grises.

Para cada problema, explicar qué error puede producir, por qué y qué debería revisarse.

## Reglas específicas
- No inventar excepciones.
- No modificar la recomendación.
- Identificar únicamente posibles errores sistemáticos derivados de su formulación y de aclaraciones validadas.
- Aplicar `core.md`.

## Al terminar
Entrega los problemas detectados sin corregir la recomendación. Si después pide otro análisis, aplica la pausa de `state.md`: los riesgos de clasificación que queden abiertos condicionan directamente cómo se definan numerador, denominador y excepciones más adelante.
