# 6 · Ficha técnica de un indicador (vía directa)

## Objetivo
A partir de una recomendación «No Hacer», construir un indicador según el enfoque elegido y elaborar su ficha técnica de forma operativa y reproducible.

## Entrada mínima
- La recomendación «No Hacer».
- El enfoque elegido: AA, SU u otro especificado.

Esta es la vía directa: no presupone haber hecho ningún análisis previo. Si el usuario no ha elegido enfoque, pregúntaselo en una frase; si no sabe cuál le conviene, ofrécele el análisis de estrategia de medición como alternativa, sin imponerlo.

## Instrucciones
- Identificar actuación y población/situación clínica.
- Construir únicamente el enfoque elegido.
- Definir numerador y denominador operativamente, con la misma unidad de análisis.
- Formular un nombre breve e inequívoco.
- Fórmula: `a × 100 / b (%)`, donde a = numerador y b = denominador.
- En Aclaraciones, definir solo términos o criterios necesarios para aplicar homogéneamente el indicador.
- Distinguir Excepciones de Exclusiones.
- Si no pueden determinarse, indicarlo.
- Señalar el tipo de fuente de datos y datos necesarios, sin inventar sistemas concretos.
- Indicar frecuencia de medición; si no puede determinarse, usar `[Propuesta]`.
- En ventana temporal, diferenciar cuando proceda periodo de medición y periodo de observación.

## Reglas específicas
Si una ambigüedad impide construir o aplicar el indicador sin modificar su sentido, numerador, denominador o unidad de análisis, señalar `[Revisar]` y explicar el motivo sin corregirlo.

## Salida
Exclusivamente tabla vertical de dos columnas `Campo | Contenido`, con filas en este orden:
1. Nombre del indicador
2. Enfoque
3. Numerador
4. Denominador
5. Fórmula
6. Aclaraciones
7. Excepciones
8. Exclusiones
9. Fuente de datos
10. Frecuencia de medición
11. Ventana temporal
12. `[Revisar]` solo si procede

## Salida en archivo
Si el usuario quiere la ficha en un documento, aplica `output/formats.md`. Formato natural: Word; PDF para adjuntar y Excel cuando vayan a manejar muchas fichas juntas.

## Al terminar
Entrega la ficha e indica qué campos han quedado como propuesta o marcados `[Revisar]`. Si después pide la ficha de expertos o el análisis de un pilotaje, aplica la pausa de `state.md`: esos dos parten de esta ficha tal cual, así que lo que aquí quede flojo se evalúa igual de flojo.
