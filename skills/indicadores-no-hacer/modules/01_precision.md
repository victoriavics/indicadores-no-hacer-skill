# 1 · Afinar la recomendación (revisión de precisión)

## Objetivo
Analizar la recomendación e identificar qué aspectos necesitan mayor precisión para poder evaluarla de forma objetiva y reproducible, evitando interpretaciones o juicios personales.

## Entrada mínima
La recomendación «No Hacer». Nada más: este análisis no presupone ningún otro.

## Instrucciones
Revisar exclusivamente estas tres dimensiones:
1. **Actuación que se pretende evitar**: valorar si queda claro qué no debe hacerse e identificar términos ambiguos.
2. **Población diana**: valorar si están suficientemente definidos los pacientes o situaciones a los que se aplica.
3. **Excepciones**: valorar si queda claro cuándo la actuación estaría justificada e identificar excepciones ambiguas, implícitas o insuficientemente definidas.

## Salida
Tabla con **exactamente tres filas**: Actuación, Población diana y Excepciones. No crear filas adicionales. Si hay varios problemas en una dimensión, agruparlos en la misma fila.

Columnas exactas:
`Elemento | Problema de precisión | Por qué puede generar ambigüedad | Qué debe concretarse / Pregunta para el equipo`

En la última columna, indicar brevemente qué debe concretarse y formular al menos una pregunta concreta que el equipo deba resolver.

## Reglas específicas
- No reformular la recomendación.
- Señalar únicamente aspectos que puedan afectar a su interpretación o medición.
- Aplicar todas las reglas de `core.md`.

## Al terminar
Entrega la tabla y cierra en abierto: qué has detectado y qué preguntas quedan para el equipo. No propongas por tu cuenta el siguiente paso salvo que el usuario lo pida.

Si después pide otro análisis, aplica la pausa de `state.md`. Aquí importa especialmente: las ambigüedades detectadas y no resueltas se arrastran hasta el indicador final.
