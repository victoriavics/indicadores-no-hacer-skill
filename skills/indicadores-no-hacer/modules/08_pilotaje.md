# 8 · Analizar un pilotaje

## Objetivo
A partir de la ficha técnica y los datos del pilotaje, evaluar la factibilidad y fiabilidad del indicador.

## Entrada mínima
- La ficha técnica del indicador, hecha aquí o aportada por el usuario.
- Datos del pilotaje cuando estén disponibles:
  - número total de casos evaluados;
  - número de casos clasificables y no clasificables;
  - motivo de los no clasificables;
  - clasificaciones independientes de los mismos casos por dos evaluadores, preferentemente caso a caso o mediante tabla de concordancia;
  - información sobre casos discordantes y sus posibles causas.

## Factibilidad
Cuando los datos lo permitan, calcular:
`Factibilidad (%) = casos en los que puede determinarse cumplimiento/incumplimiento ÷ total de casos evaluados × 100`

Identificar causas de no clasificables y valorar si se relacionan con:
- definición del criterio operativo;
- calidad/disponibilidad del registro;
- identificación de población diana o actuación;
- excepciones/exclusiones;
- otros problemas.

## Fiabilidad interobservador
Si existen clasificaciones independientes de dos evaluadores y procede metodológicamente:
- calcular coeficiente Kappa;
- presentar resultado e interpretación;
- identificar casos discordantes;
- analizar sus causas cuando haya información suficiente.

## Salida
Presentar:
`Factibilidad | Principales problemas detectados | Fiabilidad interobservador | Causas de discordancia | Aspectos a revisar antes de la implementación`

Diferenciar claramente resultados observados de propuestas de mejora.

Si el usuario quiere un archivo, aplica `output/formats.md`: el formato natural aquí es Excel, porque deja los cálculos de factibilidad y Kappa vinculados a los datos y recalculables si se añaden casos; Word o PDF si lo que quiere es el informe de resultados.

## Reglas específicas
- No inventar datos.
- No modificar automáticamente el indicador.
- Si la información es insuficiente para un cálculo o análisis, indicarlo expresamente.
- No inferir datos ausentes.

## Control de entrada
- Si faltan datos para factibilidad, no calcularla.
- Si no hay dos evaluadores independientes o no puede reconstruirse la concordancia, no calcular Kappa.
- La ausencia de datos produce una salida explícita de insuficiencia, no una estimación.

## Nota metodológica
Este análisis aporta evidencia empírica de factibilidad y reproducibilidad. Es complementario a la evaluación por expertos, no equivalente.

## Al terminar
Los problemas detectados deben revisarse antes de implementar; no modifiques el indicador por tu cuenta. Si el usuario quiere rehacer la ficha o volver a construir el indicador a partir de esto, aplica la pausa de `state.md` y parte de lo observado, no de lo supuesto.
