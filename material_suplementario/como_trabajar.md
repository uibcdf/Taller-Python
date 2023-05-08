# Cómo trabajar con este taller

Las instrucciones para generar esta web, los contenidos aquí mostrados y todo
lo relativo a este taller, se encuentra expuesto al mundo -*abierto*- y
compartido en un repositorio público de GitHub. Puedes ver su contenido siguiendo su url:
[github.com/uibcdf/Taller-Linux](https://www.github.com/uibcdf/Taller-Linux).

El propósito de tener este taller en un repositorio público en GitHub es múltiple:
- Cualquier persona puede tener acceso a él para su lectura.
- Cualquier persona puede proponer cambios y contribuir a su desarrollo.
- El repositorio se emplea al mismo tiempo para servir en internet la web de este taller.
- El repositorio permite que lo puedas copiar y editar, y publicar tus cambios.
- El repositorio es además foro de discusión y punto de encuentro para compartir dudas, problemas y soluciones.

De esta manera, el mismo repositorio es una herramienta muy útil no sólo como
vehículo de información, sino elemento interactivo para que los participantes
hagan sus pruebas, comuniquen sus dudas y problemas o contribuyan a mejorarlo.

Dado que todos los contenidos del repositorio se encuentran compartidos bajo
los términos de la licencia internacional [Creative Commons BY-NC-SA
  4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es_ES), los autores permiten que cualquier persona los
puedan copiar, distribuir, modificar y transformar libremente. Este tipo de
licencia indica a quien ejerce "estas libertades" que debe siempre respetar el
reconocimiento de la autoria de lo empleado, no puede usar el material con
fines comerciales y todo producto derivado debe compartirse en los mismos
términos. Y todo esto porque el vertiginoso desarrollo de las herramientas
computacionales abiertas primero (*Open Source*), y de los desarrollos
científicos que han adoptado mecanismos para asegurar que la ciencia sea
abierta (*Open Science*) despues, reafirman a los responsables y autores de
estos contenidos en que cooperar es más eficiente que competir a la hora de
resolver problemas que nos atañen a todos.

Vamos a ver en primer lugar cómo debes usarlo para resolver los retos semanales
y para publicar tus respuestas a las preguntas semanales.

## El repositorio como instrumento con el que interaccionar

Este taller propone que el participante cada semana resuelva unos retos y
conteste a unas preguntas relacionadas con el contenido propuesto y comentado
anteriormente. La mayoría de las ocasiones esos retos requieren la resolución
práctica de una tarea, y para que los asesores del taller podamos ayudar,
éstos, así como las respuestas a las preguntas semanales, deben ser
compartidos. ¿Y qué mejor manera de hacer todo esto si no editando tu propio
clon de este repositorio? Al fin y al cabo, si este taller forma parte de una
serie de talleres dedicada a la introducción de herramientas computacionales
para el trabajo de investigación científica, resulta muy pertinente que pongas
en práctica los principios de la ciencia abierta (*open science*) que
aprendimos del trabajo en código abierto (*open source*): para demostrar
que lo comunicado y aprendido es reproducible, todo lo necesario para
reproducirlo debe ser comunicado.

Comencemos por crear tu propio usuario en GitHub si es que todavía no tienes uno.

### Crea tu usuario en GitHub

En primer lugar debes de crear tu propio usuario en GitHub. GitHub es un
servicio gratuito... y si no lo conoces y quieres hacer trabajo científico
computacional, te va a resultar de muchísima ayuda.

[Encontrarás en esta página](otras_herramientas/github.md) las instrucciones necesarias que debes seguir para crear tu usuario.

### Haz un fork de este repositorio

Una vez que tengas tu usuario en GitHub, debes generar tu propia copia derivada
de este repositorio. O como se dice en la jerga de la comunidad del desarrollo
en colaboración de código abierto: una vez que ya tengas usuario, debes crear
tu propio "fork".

El "fork" del repositorio lo podemos entender como una copia del proyecto
original que no ha perdido el cordón umbilicar con él. Esto permite que puedas
editar y desarrollar tu propio proyecto con la posibilidad de actualizar en él
los cambios que pueda haber en el proyecto original, o que de una manera muy
"limpia" puedas proponer la incorporación de tus cambios al proyecto original
(convirtíendote a efectos de la licencia en coautor del mismo).

[Encontrarás en esta página](otras_herramientas/github.md) las instrucciones para hacer tu propio fork de este taller.

### Haz tu primer clon de tu repositorio fork

GitHub te permite interaccionar con un repositorio, en este caso con tu fork de
este taller, haciendo uso de su web con el navegador de tu máquina. Pero esto
resulta incómodo cuando vas a modificarlo y editarlo con frecuencia. ¿No sería
buena idea disponer localmente de una copia de tu fork en tu máquina? De esta
manera puedes editar un fichero en tu computadora y, cuando tu decidas, subir
los cambios a la copia de tu fork (la de la nube). A esto último se le conoce
como "empujar" los cambios, o hacer un "*push*".

[Encontrarás en esta página](otras_herramientas/github.md) las instrucciones para hacer tu primer clon local de tu repositorio.

Pero, aunque ya con tu fork local puedas cómodamente seguir el desarrollo de
este taller, no nos quedemos aquí. Imagina que terminaste de trabajar en tu
proyecto y vas a continuar en unas horas desde otra máquina, en casa, por ejemplo.
¿No sería buena idea hacer otro clon local del mismo repositorio remoto en tu
otra máquina? De esta manera, al llegar a casa descargas los cambios, haces un
"*pull*" y continuas trabajando.

### Haz tantos clones de tu repositorio como necesites

Puedes hacer tantos clones locales de tu repositorio como quieras. Sólo debes
de tener la precaución de sincronizar su contenido con el repositorio remoto
-el que GitHub almacena en la nube- antes de trabajar con ellos. Y no sólamente tu...

Vamos a suponer que trabajas con más personas en el desarrollo de un proyecto,
la escritura de un texto, por ejemplo. Habéis creado un repositorio central
(por ejemplo el que está en la nube en GiHub), y cada persona que va a
contribuir tiene sus clones locales (o su fork y sus clones locales). Git, el
motor detrás de GitHub, está perfectamente preparado para gestionar las
contribuciones de manera organizada guardando un histórico de ellas. Pero esto
es tema de otro de los talleres de la UIBCDF.

## El repositorio como foro y punto de encuentro

GitHub es un instrumento en la nube que nos permite desarrollar proyectos en
colaboración, principalmente de software y herramientas computacionales pero no
únicamente. Para facilitar la comunicación entre los desarrolladores y
también con la comunidad a la que está dirigida el proyecto, se incluyeron en
la plataforma lugares y mecanismos con los que interaccionar. Nos fijaremos
especialmente en dos: [el tablero de problemas (*Issues board*)](https://github.com/uibcdf/Taller-Linux/issues) y [el foro de
discusiones (*Discussions*)](https://github.com/uibcdf/Taller-Linux/discussions). Los usaremos para centralizar las discusiones y la
comunicación entre nosotros en este taller.

### El tablero de problemas

[El tablero de problemas (*Issues board*)](https://github.com/uibcdf/Taller-Linux/issues) fue diseñado para poder compartir:

- Propuestas de cambios e implementaciones nuevas.
- Discusiones de trabajo sobre aspectos específicos del proyecto.
- Notificaciones de problemas y errores, y propuestas de soluciones.

¿Compartir por quién y para quién? Para compartir:

- desde un miembro del equipo de desarrollo con otros miembros del equipo.
- desde cualquier usuario o miembro de la comunidad a la que va dirigido el
  proyecto al equipo de desarrollo.
- desde cualquier desarrollador a cualquier usuario o miembro de la
  comunidad que quiera interaccionar.
- desde cualquier usuario o miembro de la comunidad a otros usuarios
  o al resto de la comunidad.

En el taller vamos a provechar esta infraestructura para hacer un uso no tan
alejado de aquel para el que fue construida: interaccionar entre nosotros.

Haremos uso del tablero de problemas para compartir discusiones y dudas de
manera pública, así como para recibir comentarios y retroalimentación sobre
ellos. [En esta página](otras_herramientas/github.md) encontrarás información sobre cómo hacerlo.

Como participante del taller, el tablero de problemas debe ser tu primera
opción de contacto con el resto de participantes y con los responsables y/o
tutores. Úsala para comunicar tus problemas, dudas o propuestas.

### El foro de discusiones

Otro área de interés para interaccionar con los usuarios y desarrolladores de
un proyecto es la [web de discusiones (*Disscusions*)](https://github.com/uibcdf/Taller-Linux/discussions). Usualmente esta
herramienta se usa para centralizar conversaciones abiertas de caracter más
general que aquellas registradas en el tablero de problemas.

Usaremos el área, o foro, de discusiones para trasladar conversaciones de
interés general para los participantes, los desarrolladores de contenido y los
tutores del taller.

[En esta página](otras_herramientas/github.md) puedes encontrar indicaciones sobre cómo usar la web de discusiones.

Las discusiones que encontrarás en el taller son propuestas y moderadas por los
responsables y/o tutores. Participa en ellas libremente respetando a los demás.
Y si quieres proponer la apertura de una nueva discusión, haz uso del tablero
de problemas para comunicar la propuesta.

## El entorno de ejecución del repositorio y su material

Este taller es un proyecto en colaboración, entre los desarrolladores y
responsables del contenido, y lo más importante, entre sus participantes. Para que
dicha colaboración suceda de manera exitosa, debemos asegurar nó sólamente que
el material es público y puede ser editado por cualquier, sino que cualquiera
puede configurar el mismo entorno de trabajo para reproducirlo y modificarlo.

Para que esto se entienda mejor haremos la siguiente analogía. Imagina que
varios laboratorios científicos en el mundo que trabajan en un proyecto común,
o que simplemente trabajan sobre las mismas preguntas, necesitan compartir
hallazgos y métodos de trabajo. ¿Será suficiente con compartir un documento con
las observaciones y conclusiones hechas por unos investigadores, o un protocolo
de realización de experimento? No es suficiente para asegurar la
reproducibilidad de lo comunicado, es necesario también que las herramientas y
el entorno para reproducir el experimento sea "el mismo". Quizá esto, en
términos de "ciencia experimental" sea muy difícil o imposible, la
instrumentación será parecida pero no la misma, el equipo usado podrá ser del
mismo fabricante y el mismo modelo, pero no el mismo, y las manos del
investigador y las condiciones de laboratorio nunca serán exactamente iguales.
Pero a diferencia de la parte "experimental" de una investigación científica,
con la parte "teórica" y/o "computacional" del proyecto científico sí podemos
acercarnos a segurar la reproducibilidad de lo comunicado haciendo uso de las
mismas herramientas y el mismo laboratorio. ¿Cómo? Proporcionando instrucciones
precisas de cómo armar el entorno de ejecución, detallando las herramientas y la
versión usada. Para eso, podemos usar gestores de ambientes de trabajo como [Conda](otras_herramientas/conda.md).

El repositorio contiene un fichero llamado "conda_env.yaml" con el que puedes
configurar un entorno virtual de conda para usar las mismas herramientas que
los responsables del taller y que el resto de participantes. Y esto sin afectar
a la configuración de tu sistema operativo y el conjunto de programas que usa.

### Conda

Antes de instalar [Conda](otras_herramientas/conda.md), si es la primera vez que oyes de este gestor de
ambientes de trabajo e instalación de paquetes, imagina la siguiente situación.
Quieres reproducir un experimento computacional en tu computadora y ese
experimento fue realizado haciendo uso de las siguientes herramientas:

- Python 3.10
- MolSysMT 0.8.1 (incompatible con versiones de PyUnitWizard menores que la 1.2.0)

Pero en tu computadora tienes:

- Python 3.9
- PyUnitWizard 1.1.3

¿Debes cambiar la configuración de tu máquina? ¿Debes reemplazar tus programas
con aquellos necesarios para la ejecución del experimento? No hace falta. Conda
te permite crear entornos de trabajo como si fueran burbujas en tu máquina en
las que entrar, instalar herramientas, trabajar y salir de ellas sin afectar la
configuración de tu sistema operativo y el resto de programas.

[Encontrarás en esta página](otras_herramientas/conda.md) las instrucciones para instalar y trabajar con Conda en tu equipo.

### Crea un ambiente para trabajar en el taller

Cuando tengas instalado Conda en tu máquina de trabajo, ya puedes crear un
ambiente para trabajar con este taller haciendo uso de las mismas herramientas
que los desarrolladores y el resto de participantes. Para eso usarás el fichero
"conda_env.yaml".

Encontrarás información sobre cómo crear un entorno de trabajo con el fichero
"conda_env.yaml" en esta página.

#### Tu propia versión local de esta web

No es algo que vayas a necesitar para trabajar con este taller, pero como
prueba de que ya dispones del mismo entorno de ejecución que sus
responsables y desarrolladores, puedes compilar tu mismo estas páginas web localmente
traduciendo mediante el siguiente comando sus ficheros ".md" y ".ipynb" a
lenguaje HTML (ficheros ".html").

Activas el ambiente de trabajo -supongamos que lo llamaste "Taller-Linux"-:
```bash
conda activate Taller-Linux
```

Y en el mismo directorio de tu clon local de este repositorio, ejecuta:
```bash
make html
```

Verás que se creó un directorio nuevo llamado '\_build'. Ahora puedes lanzar con
tu navegador la web principal de este taller de manera local. Por ejemplo, si
usas Google Chrome y un sistema operativo Linux, puedes ejecutar en la
terminal:
```bash
google-chrome _build/html/index.html
```

## El material del repositorio

Para visualizar el material del repositorio, no debes de saber nada más que
navegar por las páginas y secciones de esta web. Sin embargo, para comenzar a
interaccionar con sus materiales, es necesario que comprendas la naturaleza de
sus ficheros y cómo editarlos o ejecutarlos.

Encontrarás fichero de dos tipos:
- ficheros "de texto" en lenguaje Markdown (con extensión '.md')
- fichero ejecutables llamados Jupyter notebooks o iPython notebooks (con extensión '.ipynb').

Veamos para que sirven estos dos tipos de ficheros y cómo se interacciona con ellos.

### Markdown

Uno de los lenguajes de marcado más populares para texto con formato es
Markdown. Markdown nos permite de una manera muy económica y sencilla,
especificar cómo será visualizado nuestro texto plano: en cursiva, con un
encabezado de sección, con una tabla, un hiper-enlace, una imagen... Esta misma
página web, tiene su contenido en un fichero de
texto en "lenguaje" Markdown. Échale un vistazo en esta [liga](otras_herramientas/markdown.md). Para modificar
los contenidos de esta página sólo tenemos que abrir con cualquier editor de
texto ese documento, que llamamos fuente (como si fuera la fuente de un
lenguaje de programación) y editarlo.

Con Markdown, y con otros lenguajes de marcado, entre todos convenimos una
serie de instrucciones que serán interpretadas de la misma manera por los
programas de visualiación del documento. Esto economiza mucho el trabajo y la
distribución de contenidos. Es más barato compartir por la red un texto plano
con instrucciones que un documento cuyo estilo y formato ya se encuentra
codificado en código máquina en el mismo fichero.

[En esta página](otras_herramientas/markdown.md) encontrarás más indicaciones para aprender a usar el lenguaje Markdown.

### Jupyter notebooks

Los ficheros escritos en lenguaje Markdown están escritos únicamente para la visualización y lectura de sus contenidos.
Si queremos compartir un documento en el que cualquiera puede encontrar, además de texto y recursos visuales,
instrucciones de programación y el resultado de
ellas, la libreta Jupyter notebook o IPython notebook es uno de los instrumentos adecuados.

Cuando los desarrolladores de herramientas computacionales de código libre y
los científicos que hacían trabajo computacional querían compartir código de
programación, o un experimento computacional, debían compartir por un lado el
código fuente y por otro las instrucciones y comentarios. Para después, confiar
y esperar en que el destinatario encontrara el mismo resultado y obtuviera, por
ejemplo en el caso de un experimento científico, la misma representación de los
datos producidos. Esto no hacía el trabajo en colaboración fácil.
Acudiendo al ejemplo de la parte experimental de la investigación científica,
en el ambito del laboratorio experimental los investigadores llevan siglos
definiendo la cultura y las técnicas del oficio. Una de las herramientas más
importantes que cualquiera debe manejar en este contexto es la bitácora de
laboratorio. En ella los investigadores reportan todo lo acontecido y necesario
para poder reproducir un experimento, incluso agregan las representaciones
gráficas del resultado del experimento. Todo para intentar asegurar la
reproducibilidad de lo observado. Ahora, si intentamos definir un conjunto de
hábitos y herramientas para el buen desarrollo del trabajo computacional de
investigación, nos encontramos en desventaja. Llevamos muy pocas décadas
aprendiendo y definiendo el oficio. Por ejemplo, hasta hace muy poco no
disponíamos de una libreta en la que poder construir un relato mezclando texto,
código y resultados: efectívamente, la libreta de Jupyter o el Jupyter notebook
no tiene más de una década. Es cierto que existían precedentes sobre los que
Jupyter, organización sin ánimo de lucro creada en 2014, implementó su notebook
y Jupyter Lab (lanzado en 2018).

Dicho esto, Jupyter Lab y sus Jupyter notebooks son un entorno de trabajo y un
formato de ficheros ideal para el trabajo computacional de investigación. Y por
lo mismos motivos, muy adecuados para ser el segundo soporte de contenidos que manejarás en este taller.

[En está página](otras_herramientas/jupyter.md) encontrarás indicaciones y más información sobre cómo usar
Jupyter Lab para interaccionar con los notebooks. Y con esta [otra página](otras_herramientas/notebook.md) podrás
introducirte en el uso de los notebooks.

