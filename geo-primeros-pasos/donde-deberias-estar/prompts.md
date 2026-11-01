# Prompt de apoyo

Úsalo en ChatGPT, Gemini, Claude o la IA que uses. Sustituye lo que va entre corchetes; en la herramienta sale ya relleno con tus datos.

## Sacar las preguntas de tu cliente

Para el paso 2 de la microherramienta. Adjunta el archivo de **Consultas** que exportaste de Search Console.

```text
Te adjunto las consultas de Google Search Console de la página de [PRODUCTO O SERVICIO] de mi web, [WEB]. Vendo a [TIPO DE CLIENTE] en [PAÍS O CIUDAD].

Con esas consultas, escribe las preguntas que una persona así le haría a ChatGPT sobre [PRODUCTO O SERVICIO]. En lenguaje natural y en primera persona, como las escribiría alguien real.

Reglas:
- Usa solo consultas del archivo. No te inventes temas.
- Escribe preguntas de quien quiere entender, comparar o resolver algo: qué es, cómo elegir, en qué fijarse, diferencias, cuánto cuesta, ventajas e inconvenientes.
- No pidas que te recomiende una marca o un proveedor (nada de «¿cuál me recomiendas?» o «¿cuál es el mejor?»): convierte esas consultas en preguntas sobre cómo elegir. Así la IA cita guías, comparativas, medios y foros, y no las webs de las propias marcas.
- Ignora las consultas con el nombre de mi marca, la de [WEB], aunque esté mal escrito. Si una consulta nombra a otras marcas, pregunta en qué se diferencian, sin pedir que elija una.
- Junta en una sola pregunta las consultas que signifiquen lo mismo.
- Una sola pregunta por fila.
- Añade solo el contexto que se deduce de la consulta o de a quién vendo. No inventes datos que no estén ahí, como cifras, nombres o situaciones personales.
- Si la respuesta puede cambiar según el país o la ciudad, menciona [PAÍS O CIUDAD] en la pregunta, como lo haría alguien de allí.
- Ordénalas de la más importante a la menos importante según los clics y las impresiones de sus consultas.

Devuélveme solo un CSV separado por punto y coma, con esta cabecera exacta:
Pregunta;Consulta de origen
```

Guarda la respuesta como archivo `.csv`. Si la IA te la da como texto, cópiala en un archivo de texto y guárdalo con la extensión `.csv`; no hace falta quitar lo que escriba antes o después. Después, cárgalo en la herramienta con *Importar CSV*.
