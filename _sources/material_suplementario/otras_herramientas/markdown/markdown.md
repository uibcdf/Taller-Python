
:::{figure} markdown.svg
:align: center
:::

<br>

# Markdown

## ¿Qué es Markdown?

Markdown es un lenguaje de marcado ligero que Jupyter y otros servidores como GitHub
usan para intepretar texto decorado. Se ha popularizado porque ha resultado ser
un buen consenso en cuanto a un conjunto de normas para la edición en texto plano y
así como para su traducción a texto decorado mostrado por webs y aplicaciones.
Te preguntarás, ¿por qué es esto necesario? Compartir ficheros de texto plano
escritos en un lenguaje de marcado resulta conveniente, siempre será más barato
manejar y transferir por la red ficheros de texto plano por su pequeño tamaño.

Para entender como funciona un lenguaje de marcado como Markdown, pongamos unos
ejemplos. Veamos cómo marcar texto en cursiva, negrita o ambas:

```markdown
*cursiva*
**negrita**
***cursiva y negrita***
```

*cursiva*     
**negrita**    
***cursiva y negrita***    

A continuación puedes ver cómo se escribe una tabla en Markdown:

```markdown
| item | prize | amount | total |
| ---- | ----- | ------ | ----- |
| A | 3.0 | 2 | 6.0 |
| B | 1.5 | 3 | 4.5 |
```

| item | prize | amount | total |
| ---- | ----- | ------ | ----- |
| A | 3.0 | 2 | 6.0 |
| B | 1.5 | 3 | 4.5 |

O un texto encerrado en una caja a modo de cita:

```markdown
> This is a quote
```

> This is a quote

Y por último, un enlace en este caso a otra web:

```markdown
Si quieres saber más sigue [este enlace](https://www.markdownguide.org/getting-started/).
```

Si quieres saber más sigue [este enlace](https://www.markdownguide.org/getting-started/).

## ¿Cómo se usa?

Te recomendamos que eches un vistazo a cualquiera de las webs propuestas en la
sección ["Más recursos útiles"](recursos). Encontrarás las mismas listas de
ejemplos describiendo la sintaxis. Si tuvieramos que recomendar únicamente dos,
propondríamos los siguientes enlaces. El primero por ser de John Gruber, uno de
los creadores de Markdown. El segundo por parecernos una de las guias más
completas para quien descubre Markdown por primera vez.
 
- [daringfireball.net][daringfireball]
- [markdownguide.org][markdownguide.org]

Ten en cuenta que algunos servidores o aplicaciones pueden tener sus
peculiaridades así que siempre es mejor echarle un ojo a la documentación
específica, por ejemplo de Jupyter o GitHub:

- [Working with Markdown in Jupyter Notebooks][markdown_jupyter]
- [Mastering Markdown GitHub][mastering_markdown_github]
- [Basic Markdown writing GitHub][basic_markdown_github]
- [Cheatsheet Markdown in GitHub][cheatsheed_markdown_github]
- [Markdown in GitLab][markdown_gitlab]

## Dudas, problemas técnicos y soluciones.

Para compartir con nosotros y con el resto de participantes las dudas,
problemas, sugerencias o soluciones, que pudieras tener sobre el uso de
Markdown y esta sección, te proponemos usar la siguiente discusión en este
repositorio:

- [Foro técnico sobre Markdown][discusion]

(recursos)=
## Más recursos útiles

El propósito de esta unidad es ser un documento únicamente introductorio.
Puedes encontrar -o contribuir añadiendo- más información útil en los
siguientes listados de ["Documentación"](documentacion) y ["Tutoriales, webinars
y cursos gratuitos"](tutoriales)

(documentacion)=
### Documentación

No existe una documentación oficial sobre Markdown. Lo más parecido podría ser
la web de uno de sus creadores, John Gruber:

- [daringfireball.net][daringfireball]

Échale un ojo a la siguiente sección para encontrar más recursos útiles para
aprender a usar Markdown.

(tutoriales)=
### Tutoriales, webinars y cursos gratuitos <a class="anchor" id="tutoriales"></a>

Aquí encontrarás una lista de tutoriales, videos o cursos gratuitos que puedes
visitar para aprender más sobre Mardown.

- [markdownguide.org][markdownguide.org]
- [Markdown in Carpentries-Incubator][carpentries-incubator]

[daringfireball]: https://daringfireball.net/projects/markdown
[markdownguide.org]: https://www.markdownguide.org/basic-syntax/  
[markdown_jupyter]: https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html    
[mastering_markdown_github]: https://www.markdownguide.org/
[basic_markdown_github]: https://help.github.com/articles/basic-writing-and-formatting-syntax/    
[cheatsheed_markdown_github]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet       
[discusion]: https://github.com/uibcdf/Taller-Python/discussions/10
[markdown_gitlab]: https://about.gitlab.com/handbook/markdown-guide/
[carpentries-incubator]: https://carpentries-incubator.github.io/markdown-intro/

