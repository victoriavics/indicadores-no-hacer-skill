# 7 · Ficha de evaluación por un panel de expertos

## Objetivo
A partir de la ficha técnica, preparar una ficha para que un panel de expertos evalúe el indicador, sin modificarlo ni responder en su nombre.

## Entrada mínima
La ficha técnica del indicador. Puede haberse hecho en esta conversación o traerla el usuario ya redactada. Si está incompleta en campos que los expertos necesitan valorar, dilo antes de generar el documento.

## Escala
- 1–3: valoración baja, requiere modificaciones sustanciales.
- 4–6: valoración intermedia, requiere aclaraciones o mejoras.
- 7–9: valoración alta, adecuada.

## Dimensiones
1. **Relevancia en el contexto**: frecuencia suficiente de la práctica y potencial de mejora.
2. **Validez facial**: grado en que el indicador representa adecuadamente el cumplimiento/incumplimiento de la recomendación.
3. **Factibilidad**: posibilidad de identificar reproduciblemente población diana, actuación y excepciones/exclusiones con los datos disponibles, considerando registro, codificación, vinculación y complejidad.
4. **Utilidad para la mejora**: capacidad para identificar oportunidades relevantes de mejora asistencial.

## Salida
Generar directamente el documento listo para cumplimentar. Formato natural: PDF si se imprime o se envía, Excel si se rellena en pantalla y luego se vacían las puntuaciones, Word si el equipo quiere retocarlo antes. Propón uno según lo que diga el usuario y ofrece los otros en una línea. Contenido, sea cual sea el formato:
- Encabezado breve con nombre y enfoque del indicador y escala 1–9.
- Para cada dimensión: pregunta dirigida al experto, `Puntuación: ___/9` y espacio suficiente para `Observaciones`.
- Finalizar con: `Si considera que el indicador debe modificarse, indique qué elementos cambiaría y por qué`, dejando espacio para respuesta.

## Formato
Aplicar `output/formats.md` y las reglas del formato elegido. Diseño profesional, limpio y compacto. En Word y PDF: A4, márgenes adecuados, tipografía legible, jerarquía clara, y el mínimo de páginas compatible con que se pueda escribir a gusto. En Excel, hoja de evaluación con validación de la puntuación y hoja de vaciado por experto.

## Reglas específicas
- No asignar puntuaciones.
- No responder en nombre de los expertos.
- No añadir contenido distinto del solicitado.

## Nota metodológica
Este análisis evalúa el indicador mediante juicio experto estructurado. Es complementario, no equivalente, al pilotaje empírico. Ninguno sustituye al otro.

## Al terminar
Entrega el documento y recuérdale que las puntuaciones las ponen los expertos, no tú. Si vuelve luego con las respuestas del panel y quiere rehacer la ficha técnica, aplica la pausa de `state.md`: parte de lo que dijeron los expertos, no de lo que se supone que quisieron decir.
