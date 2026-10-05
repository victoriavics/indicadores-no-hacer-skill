# 5 · Revisar los indicadores con bibliografía

## Objetivo
Revisar una tabla de indicadores y contrastarla con fuentes clínicas vigentes y de referencia.

## Entrada mínima
Una tabla de indicadores ya construida. Puede venir de un análisis anterior de esta conversación o traerla el usuario de fuera; no importa cómo se hiciera.

## Restricción estructural
Mantener intacta su estructura:
- No añadir ni eliminar filas o columnas.
- Conservar AA/SU.
- No modificar numeradores ni denominadores.

## Instrucciones
### Excepciones
- Comprobar validez.
- Añadir las relevantes que falten.
- Distinguir entre clínicas (actuación justificada) y técnicas/de codificación (posibles falsos positivos sin incumplimiento real).
- Mantener coherencia entre AA y SU cuando procedan de la misma recomendación.

### Aclaraciones
- Identificar ambigüedades de definición, terminología, criterios, umbrales, población o periodo temporal.
- Si un problema exige modificar tipo, numerador o denominador, no corregirlo: marcar `[Revisar]` y explicar el motivo.

## Fuentes
Priorizar:
1. Fuente original de la recomendación.
2. Guías y documentos oficiales de sociedades científicas.
3. Consensos, revisiones sistemáticas y metaanálisis.
4. Estudios primarios o fichas técnicas cuando sean necesarios.

Priorizar fuentes vigentes y recientes sin excluir referencias anteriores que sigan siendo aplicables. Toda adición o matiz debe citarse `[1]`, `[2]`, `[1,2]`…

## Reglas específicas
- No inventar excepciones, criterios, referencias ni DOI.
- Señalar discrepancias entre fuentes o evidencia insuficiente.
- La revisión exige consulta externa de fuentes fiables cuando sea posible.
- Aplicar `core.md`.

## Salida
- Devolver la tabla completa conservando exactamente filas y columnas.
- Marcar `[Añadido]` en la información incorporada.
- Marcar `[Revisar]` en problemas que requieran reconsideración.
- Añadir bibliografía numerada y completa.
- DOI solo si está verificado.
- En documentos institucionales: organismo, título y año.

## Formato de correcciones
El código de color es el mismo en cualquier formato: original en negro, añadidos en azul, revisiones en rojo, referencias del mismo color que el fragmento que respaldan, bibliografía en negro. Las marcas `[Añadido]` y `[Revisar]` se conservan siempre en el texto, además del color.

Si se entrega en archivo, aplica `output/formats.md` para elegir el formato y sus reglas. Aquí el formato natural es Word; PDF si va a circular sin tocarse y Excel si quieren filtrar por indicador.

## Al terminar
Lo marcado `[Revisar]` no se corrige solo: debe resolverlo el usuario o su equipo antes de consolidar una versión nueva. Dilo así de claro al entregar. Si después pide una ficha técnica o una evaluación, aplica la pausa de `state.md` recordando qué sigue en rojo.
