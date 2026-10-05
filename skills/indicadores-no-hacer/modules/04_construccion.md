# 4 · Construir los indicadores

## Objetivo
Transformar una o varias recomendaciones en los indicadores necesarios para medir su cumplimiento o incumplimiento de forma clara, reproducible y coherente.

## Entrada mínima
Una o varias recomendaciones «No Hacer». Si hay decisiones o aclaraciones validadas, incorpóralas; si no, se puede construir igualmente señalando lo que falte. No exige haber hecho los análisis anteriores.

## Instrucciones
Analizar cada recomendación independientemente.
- Puede generar AA, SU, ambos o varios indicadores si existen actuaciones, poblaciones o escenarios diferenciados.
- No generar AA y SU por sistema.
- Definir numerador y denominador operativamente y con la misma unidad de análisis.

### Aclaraciones
Incluir solo precisiones necesarias:
- En AA, priorizar cómo identificar una actuación contraria a la recomendación.
- En SU, priorizar población diana, unidad de análisis y, cuando proceda, episodio o periodo de observación.
- Mantener aclaraciones comunes cuando corresponda, sin forzarlas.

### Excepciones
- Incluir únicamente circunstancias en las que la actuación estaría justificada.
- Mantenerlas iguales en AA y SU si son comunes.
- Diferenciarlas solo por razones clínicas o metodológicas.
- No confundir excepciones clínicas con aclaraciones metodológicas.

## Reglas específicas
- No inventar criterios, indicaciones, excepciones, poblaciones, definiciones, ventanas temporales ni puntos de corte no deducibles del texto o de aclaraciones validadas.
- Si falta información, indicarlo.
- Si las excepciones no están especificadas, señalar que deben consultarse en la recomendación completa o su fuente original.
- Aplicar `core.md`.

## Salida por defecto del módulo
Resultado estructurado con las columnas:
`Recomendación | Tipo | Numerador | Denominador | Aclaraciones | Excepciones`

## Salida en archivo
Cuando el usuario pida un documento, genéralo directamente y aplica `output/formats.md`. Para una tabla de indicadores, el formato natural es Excel si el equipo va a seguir trabajando sobre ella, y Word o PDF si es para un documento o para circular: propón uno y menciona en una línea que puedes darlo en los otros.

Si la petición era directamente el archivo, no vuelques antes la tabla completa en la conversación.

## Al terminar
Entrega la tabla y señala qué ha quedado sin poder concretarse. Si después pide una revisión bibliográfica, una ficha técnica o una evaluación, aplica la pausa de `state.md`: cualquier ambigüedad de numerador, denominador o unidad de análisis se propagará a esos documentos.
