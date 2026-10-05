# Reglas de salida Excel

El Excel no es una copia de la tabla de Word: es una hoja con la que el equipo va a trabajar. Debe poder filtrarse, ordenarse y ampliarse sin romperse.

## Principios generales
- Una fila = un registro real (un indicador, un caso del pilotaje, una respuesta de un experto). Nunca celdas combinadas en la zona de datos: rompen filtros y ordenaciones.
- Fila 1 de encabezados, en negrita y con relleno suave; inmovilizar paneles bajo el encabezado y activar filtro automático.
- Anchos de columna ajustados al contenido y ajuste de texto activado en las columnas largas (numerador, denominador, aclaraciones, excepciones); alineación superior izquierda.
- Una hoja por tipo de contenido, con nombre explícito (`Indicadores`, `Datos`, `Resultados`, `Bibliografía`). Nada de `Hoja1`.
- Columnas de texto largo formateadas como texto, para que Excel no reinterprete códigos ni fechas.
- Si un dato no se conoce, se deja la celda vacía y se explica en la columna de observaciones. No se rellena con ceros, guiones ni estimaciones.
- Las marcas `[Añadido]`, `[Revisar]` y `[Propuesta]` se conservan en el texto de la celda, además del color.

## Tabla de indicadores
Columnas, en este orden:
`Recomendación | Tipo | Numerador | Denominador | Aclaraciones | Excepciones`

- Una fila por indicador. Si una recomendación genera varios, se repite el texto de la recomendación en cada fila en lugar de combinar celdas: así se puede filtrar por recomendación.
- Añadir delante una columna `Id` correlativa para poder referirse a cada indicador sin ambigüedad.
- Si hay varias recomendaciones, van todas en la misma hoja.
- Opcionalmente, separar visualmente los bloques de una misma recomendación con un borde superior más marcado; nunca con filas en blanco.

## Revisión clínica y bibliográfica
- Se conserva la tabla original con exactamente sus filas y columnas, y se añaden al final las columnas `Añadido`, `Revisar` y `Referencias`.
- El texto original no se toca. Lo incorporado va en azul, lo marcado `[Revisar]` en rojo, dentro de sus columnas.
- Hoja aparte `Bibliografía` con las referencias numeradas y completas, en negro, con la misma numeración que se cita en las celdas.

## Ficha técnica
- Dos columnas, `Campo | Contenido`, con los campos en el mismo orden que en el módulo.
- Si hay varias fichas, una hoja por indicador con el nombre del indicador abreviado, o bien una sola hoja con un indicador por columna cuando se quieran comparar.

## Ficha del panel de expertos
Dos hojas:
- `Evaluación`: una fila por dimensión, con las columnas `Dimensión | Pregunta | Puntuación (1-9) | Observaciones`. La columna de puntuación con validación de datos de 1 a 9 y bloqueada al resto de valores. Al final, la fila de la pregunta abierta sobre modificaciones. Encabezado con nombre y enfoque del indicador y la escala.
- `Vaciado`: una fila por dimensión y una columna por experto (`Experto 1`, `Experto 2`…), con mediana y rango por dimensión calculados con fórmula. Las celdas de los expertos se dejan vacías: las puntuaciones no las pones tú.

## Pilotaje
Tres hojas:
- `Datos`: una fila por caso, con las columnas `Id caso | Clasificable (Sí/No) | Motivo si no clasificable | Evaluador 1 | Evaluador 2 | Discordante | Causa de la discordancia`. Solo con los datos que el usuario haya aportado; los casos que no existan no se inventan.
- `Resultados`: factibilidad, concordancia observada y Kappa, calculados con fórmulas que apunten a `Datos`, de modo que se recalculen si el equipo añade casos. Junto a cada resultado, su interpretación en texto.
- `Revisar`: problemas detectados y aspectos a resolver antes de la implantación, separando lo observado de las propuestas de mejora.

Si faltan datos para un cálculo, la celda del resultado queda vacía con una nota explicando qué falta. No se calcula Kappa sin dos clasificaciones independientes.

## Colores
Los mismos criterios que en Word: original en negro, añadidos en azul, `[Revisar]` en rojo, bibliografía en negro. En Excel el color va en la fuente, no en el relleno; el relleno se reserva para encabezados.
