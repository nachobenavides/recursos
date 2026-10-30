# Prompts de apoyo

Úsalos en ChatGPT, Gemini, Claude o la IA que uses. Sustituye lo que va entre corchetes; en la herramienta, el prompt 1 sale ya relleno con tus datos.

## Prompt 1 · Sacar las preguntas de tu cliente

Para el [paso 2](guia.md#paso-2--saca-las-preguntas-de-tu-cliente). Adjunta el archivo de **Consultas** que exportaste de Search Console.

```text
Te adjunto las consultas de Google Search Console de la página de [PRODUCTO O SERVICIO] de mi web, [WEB]. Vendo a [TIPO DE CLIENTE] en [PAÍS O CIUDAD].

Con esas consultas, escribe las preguntas que una persona así le haría a ChatGPT sobre [PRODUCTO O SERVICIO]. En lenguaje natural y en primera persona, como las escribiría alguien real.

Reglas:
- Usa solo consultas del archivo. No te inventes temas.
- Incluye tanto las de quien está eligiendo qué comprar (mejor, precio, opiniones, comparativas, alternativas) como las de quien quiere entender o resolver algo relacionado (qué es, cómo se hace).
- Ignora las consultas con el nombre de mi marca, la de [WEB], aunque esté mal escrito. Las que nombran a otras marcas sí valen.
- Junta en una sola pregunta las consultas que signifiquen lo mismo.
- Una sola pregunta por fila.
- Añade solo el contexto que se deduce de la consulta o de a quién vendo. No inventes detalles como un presupuesto concreto o el proveedor que tienen ahora.
- Menciona [PAÍS O CIUDAD] cuando la respuesta pueda cambiar según dónde se compre.
- Como máximo, 8 preguntas, de la más importante a la menos importante según los clics y las impresiones de sus consultas. Si hay pocas consultas que valgan, escribe menos preguntas.

Devuélveme solo un CSV separado por punto y coma, con esta cabecera exacta:
Pregunta;Consulta de origen
```

Guarda la respuesta como archivo `.csv`. Si la IA te la da como texto, cópiala en un archivo de texto y guárdalo con la extensión `.csv`; no hace falta quitar lo que escriba antes o después. Después, cárgalo en la herramienta con *Importar CSV*.

## Prompt 2 · Analizar una web citada

Para el [paso 4](guia.md#paso-4--analiza-las-webs-que-más-se-repiten). Hazlo con la búsqueda en la web activada.

```text
Analiza esta página: [URL]

Vendo [PRODUCTO O SERVICIO] y mi competencia es [COMPETIDORES]. Dime:
1. Qué tipo de contenido es (comparativa, guía, reseña, lista de recomendados u otro) y de qué fecha.
2. Qué marcas menciona y qué dice de cada una.
3. A qué páginas de esas marcas enlaza, con la URL exacta.
4. Quién lo firma.

Si algo no aparece en la página, dilo. No lo supongas.
```

Comprueba los enlaces abriendo la página: la IA puede equivocarse con las URL.
