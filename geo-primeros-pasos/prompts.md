# Prompts de apoyo

Úsalos en ChatGPT, Gemini, Claude o la IA que uses. Sustituye lo que va entre corchetes.

## Prompt 1 · Sacar las preguntas de tu cliente

Para el [paso 2](guia.md#paso-2--saca-las-preguntas-de-tu-cliente). Adjunta el archivo de **Consultas** que exportaste de Search Console.

```text
Te adjunto las consultas de Google Search Console de la página de [PRODUCTO O SERVICIO] de mi web. Vendo a [TIPO DE CLIENTE] en [PAÍS O CIUDAD].

Con esas consultas, escribe las preguntas que haría una persona a ChatGPT antes de comprar: en lenguaje natural, en primera persona y con el contexto que daría alguien real (para qué lo quiere, su presupuesto, su situación).

Reglas:
- Usa solo consultas del archivo. No te inventes temas.
- Ignora las consultas que llevan el nombre de mi marca.
- Junta las consultas que signifiquen lo mismo en una sola pregunta.
- Da prioridad a las consultas con más clics e impresiones.
- Como máximo, 15 preguntas.

Devuélveme solo un CSV, sin texto antes ni después, separado por punto y coma, con esta cabecera exacta:
Pregunta;Consulta de origen
```

Guarda la respuesta como archivo `.csv`. Si la IA te la da como texto, cópiala en un archivo de texto y guárdalo con la extensión `.csv`. Después, cárgalo en la herramienta con *Importar CSV*.

## Prompt 2 · Analizar una web citada

Para el [paso 4](guia.md#paso-4--analiza-las-webs-que-más-se-repiten). Hazlo con la búsqueda en la web activada.

```text
Analiza esta página: [URL]

Vendo [PRODUCTO O SERVICIO] y mi competencia es [COMPETIDORES]. Dime:
1. Qué tipo de contenido es (comparativa, guía, reseña, lista de recomendados u otro) y de qué fecha.
2. Qué marcas menciona y qué dice de cada una.
3. A qué páginas de esas marcas enlaza, con la URL exacta.
4. Quién lo firma y si hay una forma de contacto visible.
5. Qué podría aportar yo para que tuviera sentido incluirme: datos, una página mejor, producto para probar o una corrección.

Si algo no aparece en la página, dilo. No lo supongas.
```

Comprueba los enlaces abriendo la página: la IA puede equivocarse con las URL.
