
:::{figure} Git-Logo-2Color.png
:align: center
:width: 20%
:::

<br>

# Git

## ¿Qué es Git?

[Git][git] es una herramienta de [control de
versiones][acerca_control_versiones]. Estas herramientas fueron concebidas para
el desarrollo de software, ya que permiten un flujo de trabajo eficiente al
mantener un historial de cambios y versiones anteriores. Más especificamente
Git fue creada por Linus Torvalds para gestionar el desarrollo de los kernels
(nucleos del sistema) de Linux. Existen otras herramientas similares, como SVN
de la cual quizás hayas escuchado o usado, no obstante hoy en dia Git se ha
convertido en un protocolo muy popular para el desarrollo de cualquier proyecto
que involucre la participación de varias personas.

¿Cómo funciona exactamente? El historial que comentamos anteriormente es el
"corazón" de Git, pues incluye: qué cambios hizo quién o cúando, así como el
propósito de los mismos. Tener dicho registro ofrece varias ventajas, pues
facilita cosas como: ir hacia atrás en la historia del desarrollo del proyecto,
implementar nuevos cambios de manera tentativa, trazabilidad de errores, crear
copias del proyecto en las que hacer pruebas para posteriormente fusionar la
copia con el proyecto original, etc.

Por esta razón, para la comunidad científica (especialmente la que desarrolla
trabajo computacional), Git se ha convertido en una manera cómoda y
relativamente flexible de gestionar tareas en grupo. Justo por eso, Git ya no
se limita únicamente al desarrollo de software. Puedes desde escribir un
documento en colaboración hasta desarrollar unos scripts de análisis o crear
una figura. En resumen, Git es un controlador de cambios que se encuentra
detrás de muchas de las tareas que realizamos individualmente y en grupo los
investigadores. Así que vale la pena presentar algunos aspectos generales sobre
su uso.


## ¿Cómo se instala?

### Git en Linux

Para instalar Git en Linux, sigue los pasos que se te sugieren desde su [sitio web oficial][git_linux].
Por ejemplo, si tu distribución es **Ubuntu**, sigue estos pasos:

1. Abre la terminal de Ubuntu presionando Ctrl + Alt + T en tu teclado.

2. Actualiza la lista de paquetes de Ubuntu con el siguiente comando:

```bash
sudo apt-get update
```

3. Instala Git con el siguiente comando:

```bash
sudo apt-get install git
```

4. Después de ingresar el comando, se te pedirá que confirmes la instalación.
   Ingresa "Y" (o "yes") y presiona Enter para continuar.

5. Espera a que se complete la instalación. Una vez finalizada, puedes
   verificar si Git está instalado correctamente ingresando el siguiente
   comando:

```bash
git --version
```

Ten en cuenta que Git suele estar por defecto instalado en cualquier
distribución de Linux, así que tal vez deberías empezar por el final.

### Git en macOS

Para instalar Git en macOS, sigue los pasos que se te sugieren desde su [sitio web oficial][git_macos].
Por ejemplo, para una distribución Homebrew:

1. Abre la aplicación "Terminal" en tu Mac. Puedes encontrarla en la carpeta
   "Utilidades" dentro de "Aplicaciones".

2. Instala Homebrew si aún no lo has hecho. Homebrew es un gestor de paquetes
   muy popular para macOS. Puedes instalar Homebrew con el siguiente comando en
   la terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

3. Una vez que se complete la instalación, actualiza la lista de paquetes de
   Homebrew con el siguiente comando:

```bash
brew update
```
	
4. Ahora puedes instalar Git con el siguiente comando:

```bash
brew install git
```

5. Después de ingresar el comando, se te pedirá que confirmes la instalación.
   Ingresa "Y" (o yes) y presiona Enter para continuar.

6. Espera a que se complete la instalación. Una vez finalizada, puedes
   verificar si Git está instalado correctamente ingresando el siguiente
   comando:

```bash
git --version
```
	
Si Git se instaló correctamente, la terminal debería mostrarte la versión de Git.

### Git en Windows

Para instalar Git en Windows, sigue los siguientes pasos :

1. Visita la página oficial de descargas de Git en el [sitio web de
   Git][git_windows].

2. Descarga el instalador de Git para Windows haciendo clic en el botón
   "Download for Windows" (Click here to download para descargar la versión
   más reciente (2.40.1) de 64 bits de Git para Windows).

3. Ejecuta el archivo de instalación descargado. Si se te solicita permiso para
   permitir que el archivo realice cambios en tu dispositivo, haz clic en "Sí"
   para continuar.

4. En la ventana de inicio de Git, haz clic en "Next" (Siguiente).

5. Lee y acepta los términos de la licencia de Git. Luego, haz clic en "Next"
   (Siguiente).

6. Elige la ubicación donde deseas instalar Git. Puedes dejar la ubicación
   predeterminada o seleccionar otra carpeta. Luego, haz clic en "Next"
   (Siguiente).

7. Selecciona los componentes que deseas instalar. La mayoría de los usuarios
   pueden dejar los componentes predeterminados seleccionados. Luego, haz clic
   en "Next" (Siguiente).

8. Elige el editor de texto que deseas utilizar con Git. Puedes elegir entre el
   editor predeterminado, Nano, o elegir otro editor. Luego, haz clic en "Next"
   (Siguiente).

9. Selecciona el "PATH environment" que deseas utilizar con Git. La opción
   predeterminada es la recomendada para la mayoría de los usuarios. Luego, haz
   clic en "Next" (Siguiente).

10. Selecciona cómo deseas que se manejen los finales de línea. La opción
    predeterminada es la recomendada para la mayoría de los usuarios. Luego,
    haz clic en "Next" (Siguiente).

11. Selecciona si deseas crear accesos directos para Git en el escritorio y en
    el menú de inicio. Luego, haz clic en "Next" (Siguiente).

12. Haz clic en "Install" (Instalar) para comenzar la instalación de Git.

13. Espera a que se complete la instalación. Una vez finalizada, haz clic en
    "Finish" (Finalizar).

14. Verifica que Git se instaló correctamente abriendo el símbolo del sistema
    (o PowerShell) y escribiendo el siguiente comando:

```bash
git --version
```

La terminal debería mostrarte la versión de Git que se instaló.

## ¿Cómo se usa?


:::{figure} xkcd_git.png
:align: center
:width: 40%
:::
    
### Como controlador de versiones local y personal

¿Quieres generar un proyecto y llevar tu propio control de versiones?
Encuentra aquí una lista de acciones que puedes usar.

Cómo crear un proyecto/repositorio:

```bash
git init
```

Cómo clonar un proyecto existente en tu máquina:

```bash
git clone /path/to/repository
```

También puedes clonar un proyecto que se encuentra en una máquina remota.

```bash
git clone username@host:/path/to/repository
```

Cómo añadir un nuevo fichero al listado de ficheros del proyecto que controla Git:

```bash
git add <filename>
```

Cómo añadir todos los ficheros presentes en el directorio al listado que
controlado Git:

```bash
git add *
```

Recordarás que comentamos sobre los registros de Git, ahora lo veremos en
acción. Primeramente veremos el comando status: 

```bash
git status
```

Notarás que Git nos menciona que estamos al día con la versión master, eso
quiere decir que la copia local y la copia en Git son idénticas. En caso
contrario se nos muestran los archivos de los cuales Git no lleva registro (si
no existen) o aquellos en los que la copia local y el master no coinciden. Por
ejemplo, crea un nuevo documento en el repositorio git y repite el comando
anterior:

```bash
touch nuevo.txt

git status
```

Ahora, supongamos que este archivo será un cambio a implementar en el
repositorio, lo que sigue es notificar a Git que estos cambios serán
"permanentes". A esta acción se la denomina "comprometer" (*commit* en inglés)
los cambios, y se realiza para registrar en el histórico el estado actual del
proyecto. Junto a estos cambios se recomienda incluir un mensaje de texto
explicando las modificaciones:

```bash
git commit -m "Commit message"
```

:::{figure} xkcd_git_commit.png
:align: center
:width: 60%
:::

Procura que tus notas sobre los commits sean claras, así aprovecharás al máximo
el registro de Git y te ahorrarás dolores de cabeza en el futuro.

Cabe mencionar que notificar los cambios no es suficiente para implementarlos.
Si cuentas con los permisos adecuados, despues de haber hecho el
correspondiente `commit`, es necesario "empujar" tus cambios al repositorio
remoto, mediante el siguiente comando:

```bash
git push
```

Durante el uso personal, el comando push casi no te dará algun error a menos
que pierdas conexión con Git. Cuando se trabaja en colaboración es posible que
haya cambios en el repositorio remoto, en ese caso Git evitará que implementes
cambios si no posees la versión "más actual". Para resolver esta situación
puedes "tirar" de estos para implementarlos en tu clon:

```bash
git pull
```

Después de esto, podrás revisar los cambios implementados y decidir antes de
duplicar o implementar de forma innecesaria. Recuerda, el comando pull sirve
para mantener al día tu clon local, por lo que una buena práctica de trabajo es
"tirar" del repositorio antes de intentar implementar cambios.

En la introducción comentamos también que Git permite hacer pruebas al margen
de la copia principal. Para realizar dicha operación haremos uso de los
siguientes comandos:

```bash
git checkout -b nombre_de_la_rama # para crear la rama
git checkout master # para volver a la copia maestro
git branch -d nombre_de_la_rama # para borrar la rama
git merge nombre_de_la_rama # para fusionar los cambios de una rama en la copia maestra
```

Encuentra un breve listado de otros comandos útiles [aquí][guia_sencilla]

### Como servidor remoto central de git

#### En un servidor tuyo

Puedes configurar Git en un servidor central al que otras máquinas pueden tener
acceso. La UIBCDF tiene su servidor de Git central configurado, pero la
información e instrucciones para configurarlo escapan al propósito de este
documento.

#### En la nube

Si no cuentas con una máquina que poder configurar como servidor, puedes hacer
uso de servidores remotos en la nube como por ejemplo GitHub o GitLab.
Para hacer uso de GitHub, o interaccionar desde tu máquina con un repositorio
de GitHub, te sugerimos acudas a la página ["GitHub"][otras_herramientas_github] de este taller.

### Breve compendio de los comandos más útiles

#### Listado de ramas

Para listar únicamente las ramas locales:

```bash
git branch
```

Para listar únicamente las ramas remotas:

```bash
git branch -r
```

Para listar todas las ramas:

```bash
git branch -a
```

#### Cambio de rama

```bash
git checkout nombre_de_rama
```

#### Listado de ramas y commits

Para listar únicamente las ramas locales:

```bash
git show-branch
```

Para listar únicamente las ramas remotas:

```bash
git show-branch -r
```

Para listar todas las ramas:

```bash
git show-branch -all
```

#### Creación de nueva rama

Para crear una nueva rama en el repositorio local

```bash
git branch nombre_de_rama
```

Podemos tambien crear una nueva rama y saltar a ella con un solo comando:

```bash
git checkout -b nombre_de_rama
```

En el caso de que exista un clon remoto del repositorio podemos empujar la
creación de la nueva rama. Por ejemplo, supongamos que nuestro repositorio
original es remoto, podemos empujar la creación de nuestra nueva rama local
como:

```bash
git push -u origin <new-branch>
```

#### Eliminación de una rama

Para eliminar una rama:

```bash
git branch -d nombre_de_rama
```

#### Creación del clon local de un una nueva rama remota

Supongamos que en el repository remoto denominado 'origin' hay una rama llamada
'foo'. Esto se puede ver de la siguiente manera:

```bash
git branch --all

  gh-pages
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/foo
  remotes/origin/gh-pages
  remotes/origin/master
```

Podemos traer al clon local del repositorio la copia de la rama 'foo':

```bash
git fetch origin foo:foo
```

Ya podemos ver que existe la rama local 'foo':

```bash
git branch --all

  foo
  gh-pages
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/foo
  remotes/origin/gh-pages
  remotes/origin/master
```

Y podemos también cambiar a la nueva rama para trabajar localmente:

```bash
git checkout foo
```

### Compendio de las rutinas más útiles

#### Creo una nueva rama y la empujo también al origin remoto

```bash
gir checkout -b nombre_de_rama
git push -u origin nombre_de_rama
```


## Dudas, problemas técnicos y soluciones

Para compartir con nosotros y con el resto de participantes las dudas,
problemas, sugerencias o soluciones, que pudieras tener sobre el uso de
Git y esta sección, te proponemos usar la siguiente discusión en este
repositorio:

- [Foro técnico sobre Git][foro_tecnico_git]

## Más recursos útiles

Esta web era sólo una guia introductoria. No es funcional documentarse o
estudiar mucho sin antes probar a instalar y usar la herramienta. Aprenderás de
manera más solida si con el uso te van surgiendo necesidades a las que vas
dando solución poco a poco. Puedes encontrar -o contribuir añadiendo- más
información útil en los siguientes listados.

### Documentación

Compartimos en esta sección la documentación oficial de la herramienta:

- [Git][git_docs]
- [Pro Git Book (español)][pro_git_book_es]
- [Pro Git Book (inglés)][pro_git_book_en]

### Tutoriales, Webinars y cursos gratuitos

Aquí encontrarás una lista de tutoriales, videos o cursos gratuitos que puedes
visitar para aprender más sobre Git.

- [Git desde GitHub][git_desde_github]
- [La guia sencilla][guia_sencilla]
- [Software Carpentry - El controlador de versiones con Git][swcarpentry]
- [Atlassian Git Tutorials][atlassian]
- [Git vs. GitHub][git_vs_github]
- [Git-Tower Learn][git_tower_learn]
- [MOLSSI Git and GitHub][molssi]
- [Coursera: Git][coursera_git]


[otras_herramientas_github]: ../github/github.md 
[git]: https://git-scm.com/
[git_linux]: https://git-scm.com/download/linux
[git_macos]: https://git-scm.com/download/mac
[git_windows]: https://git-scm.com/download/win
[acerca_control_versiones]: https://git-scm.com/book/es/v1/Empezando-Acerca-del-control-de-versiones
[foro_tecnico_git]: https://github.com/uibcdf/Taller-Python/discussions/6
[pro_git_book_es]: https://git-scm.com/book/es
[pro_git_book_en]: https://git-scm.com/book/en
[git_docs]: https://git-scm.com/docs  
[guia_sencilla]: http://rogerdudler.github.io/git-guide/index.es.html
[swcarpentry]: https://swcarpentry.github.io/git-novice-es/
[atlassian]: https://www.atlassian.com/git/tutorials
[git_tower_learn]: https://www.git-tower.com/learn/    
[git_vs_github]: https://jahya.net/blog/git-vs-github/      
[molssi]: https://education.molssi.org/python-package-best-practices/00-git-and-github.html
[git_desde_github]: https://docs.github.com/es/get-started/getting-started-with-git
[coursera_git]: https://www.coursera.org/learn/git-espanol


