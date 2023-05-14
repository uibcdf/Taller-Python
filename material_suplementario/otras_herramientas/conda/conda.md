
:::{figure} conda_logo.svg
:align: center
:::

<br>

# Conda

Esta introducción a Conda está pensada para aquellos que tienen poco o ningún
conocimiento previo. Esperamos pueda serte útil.

## ¿Qué es Conda?

Conda es un gestor de entornos o ambientes de trabajo, paquetes y canales, operativo para varios
lenguages de programación -originalmente fue creado para Python- y sistemas operativos como
Windows, macOS o Linux. Antes de nada, aclaremos qué es un paquete, qué es un canal y qué es un
entorno. 

### ¿Qué es un paquete?

Un paquete (o librería) es un conjunto de ficheros de código 'empaquetado' con las instrucciones de
instalación pertinentes y programado para realizar unas tareas específicas. Si estuvíeramos
hablando de un lenguage compilado, el paquete sería el 'programa' junto con su instalador que
compilas (instalas) en tu computadora. Este programa suele requerir para su correcto funcionamiento
que en tu computadora tengas otros programas instalados -dependencias-. Así, es habitual que antes
de instalar un programa tengas que preocuparte de que las dependencias estén presentes. Por
ejemplo, el sistema operativo Linux cuenta con gestores de paquetes con los que instalas software
nuevo en tu computadora: 'apt-get', 'yum', 'synaptic', 'aptitude', etc -según la distribución que
estés usando-. Estos gestores se preocupan por ti de que el software que quieres instalar encuentre
las dependencias en tu máquina o las descargue del repositorio apropiado para su instalación.

Si tuvieras que instalar a mano el software que necesitas y sus dependencias -colocando cada cosa
donde debe ir en tu sistema operativo-, con el paso del tiempo el número de problemas a resolver
para instalar programas nuevos o para que éstos funcionen correctamente haría el mantenimiento de
tu máquina muy laborioso. Es muy conveniente que un gestor mantenga el equilibrio en el ecosistema
de paquetes instalados en tu computadora.

### ¿Qué es un canal?

Un grupo de desarrolladores o usuarios pueden configurar una lista de paquetes para ser descargados
en red por cualquiera, de manera pública o privada, haciendo uso del gestor de paquetes. A este
repositorio de software se le conoce como 'canal' (el 'canal' para conda es similar a lo que
entendemos como 'repositorio' en Linux).

Como ejemplo de canal público de conda puedes echarle un ojo a, probablemente, el
canal más popular mantenido por usuarios: [conda-forge][conda_forge] y [su
lista de más de 21,700 paquetes][anaconda_conda_forge].

### ¿Qué es un entorno?

Imagina la siguiente situación:

- Debes instalar la librería 'A' en su última versión 1.2.4 que depende de versiones mayores a la
  2.0.0 de la librería 'B'.
- En tu máquina tienes instalada la versión 1.6.5 de la librería 'B'.
- Las versiones de 'B' mayores que 2.0.0 trabajan con Python 3.9, 3.10 y 3.11. Pero la versión de
  Python que encuentras en tu máquina es la 3.8.

Es decir, para instalar la versión que necesitas de 'A' encuentras incompatibilidades con tu
versión de 'B' y Python. ¿Qué puedes hacer? Puedes actualizar la versión de Python de tu sistema
operativo a por lo menos la versión 3.9. Pero tendrás que asegurar que todo el software que ya
tienes instalado sea compatible con la nueva versión de Python 3.9, o tendrás que actualizarlo
-esperando que para cada programa encuentres un reemplazo adecuado-. Así, por ejemplo, la librería
'B' se actualizará a una versión mayor que la 2.0.0 para que puedas instalar 'A'. Pero espera un
momento... ¿serán el resto de programas que había en tu máquina haciendo uso de 'B' compatibles con
la nueva versión? La situación se complica...

¿Qué te parecería tener una herramienta para crear un entorno, o un ambiente (*environment*),
aislado en tu computadora para instalar la versión 1.2.4 'A' y todas sus dependencias sin afectar
al resto de programas y a tu sistema operativo? Un gestor de entornos o ambientes de trabajo como
Conda puede hacer eso por ti.

Un entorno (o ambiente -`environment`-) de trabajo o de desarrollo es a todos los efectos como una burbuja dentro de tu
computadora. La activas, y puedes instalar en ella una lista de paquetes que podrás usar únicamente
cuando estés dentro de la burbuja (con el ambiente activado). Esos paquetes son los primeros que
encontrará tu usario al trabajar en el ambiente, pero no los únicos. Si quieres usar la herramienta
'A' y no la instalaste en el entorno pero si está en el sistema, tu usuario tiene acceso a la 'A'
del sistema sin que tengas que hacer nada. Ahora, si en el sistema tienes la versión '1.1.3' y
necesitas usar la '1.2.4'... con el ambiente activo puedes instalar dicha versión y
todas sus dependencias. Al estar en un entorno de conda, tu usuario da preferencia a las
herramientas instaladas en dicho entorno. Ya puedes usar la versión '1.2.4'. Y cuando salgas de la
burbuja (cuando desactives el entorno) volverás a usar la versión '1.1.3' que había en tu máquina
junto con el sistema operativo.

### ¿Qué es entonces un gestor de entornos, paquetes y canales?

Un gestor de entornos, paquetes y canales, como pueden ser conda, homebrew, pip
o pipenv, se ocupa de administrar tus entornos de trabajo posibilitando en
ellos la instalación y actualización de paquetes desde los canales que
configures sin que se produzcan incompatibilidades entre ellos, sus dependencias, y el software que
tienes instalado en la computadora junto a tu sistema operativo.

Conda, creado y soportado por [Anaconda][anaconda], ofrece esto y más. La mejor
manera de comenzar para un usuario inexperto es instalar la última versión de
miniconda y empezar a usarlo.

<br>
<center>
<img src="https://www.explainxkcd.com/wiki/images/c/cb/python_environment.png" width="400">
</center>
<br>

### ¿Qué es Miniconda?

[Miniconda][miniconda] es la versión 'mínima' de Conda con la que se aconseja empezar. Conda
ofrece descargar un gestor junto con una gran colección de librerías, pero esto
además de pesado es innecesario. Instala miniconda en tu máquina para comenzar
con el uso de conda y descarga poco a poco los paquetes que vayas requiriendo.

## ¿Cómo se instala?

Puedes encontrar las instrucciones de instalación y manejo de conda en [su
página oficial][conda_docs]. Antes de ver las instrucciones según el sistema
operativo que uses, échale un ojo al menos a la estructura de la [guía de
usuario][conda_user_guide].

:::{hint}
Te sugerimos instalar Miniconda, no Anaconda.
:::

### Linux.

Sigue el siguiente enlace para encontrar las instrucciones de instalación para Linux dadas en la web
de documentación oficial de conda:

- [Cómo instalar conda en Linux.][install_conda_linux]

### macOS.

Sigue el siguiente enlace para encontrar las instrucciones de instalación para macOS dadas en la web
de documentación oficial de conda:

- [Cómo instalar conda en macOS.][install_conda_macOS]

### Windows.

Sigue el siguiente enlace para encontrar las instrucciones de instalación para Windows dadas en la web
de documentación oficial de conda:

- [Cómo instalar conda en Windows.][install_conda_windows]

## ¿Cómo se usa?

Existe una excelente [documentación oficial][conda_user_guide] con [breves guías para
comenzar][conda_getting_started] y [*cheat sheets*][conda_cheat_sheets].

Vamos a exponer aquí la pequeña lista de comandos que probablemente más vas a usar.

### Cómo actualizar conda

Puedes actualizar el mismo conda con el siguiente comando:

```python
conda update conda
```

### Cómo crear un entorno

Cómo crear un entorno de python 3 llamado en este caso `taller`:

```python
conda create -n taller python=3
```

Para crear un entorno a partir de un fichero '\*.yaml', supongamos que se llama
'conda_env.yaml', con la lista de canales y paquetes necesarios:

```python
conda env create -n taller -f conda_env.yaml
```

### Cómo activar un entorno:

Puedes cargar o activar un entorno así:

```bash
conda activate taller
```

### Cómo instalar un paquete en un entorno:

Para instalar un paquete, por ejemplo `numpy`,  en un entorno debes de ejecutar el siguiente comando (con el entorno
activo):

```bash
conda install numpy
```

Si necesitas instalar un paquete de un canal específico, por ejemplo `jupyterlab` del canal
`conda-forge`, puedes ejecutar el comando:

```bash
conda install -c conda-forge jupyterlab
```

### Cómo actualizar los paquetes de un entorno

Debes activar el entorno que quieres actualizar y hacer uso del comando:

```bash
conda update --all
```

### Cómo consultar los paquetes de un entorno

Para consultar la lista de paquetes instalados en un entorno, con el entorno activo:

```bash
conda list
```

### Cómo desactivar un entorno

Para desactivar el entorno activo:

```bash
conda deactivate
```

### Cómo consultar la lista de entornos

Puedes consultar la lista de entornos disponibles con:

```bash
conda info --envs
```

### Cómo eliminar un entorno

Cómo eliminar un entorno:

```bash
conda env remove --name taller
```

### Cómo añadir un canal

Puedes configurar tu conda para que siempre busque y comprueba paquetes en un canal que no viene
incluido por defecto en tu instalación. Para eso, suponiendo que quisieras añadir el canal
`conda-forge`, ejecuta el siguiente comando:

```
conda config --add channels conda-forge
```

### Cómo consultar la lista de canales

Para consultar la lista de canales incluidos en tu archivo de configuración y su prioridad:

```bash
conda config --get
```

### Cómo eliminar un canal

Puedes eliminar un canal, en este caso `conda-forge`, de la lista de canales
incluidos en tu archivo de configuración.

```bash
conda config --remove channels conda-forge
```

---

## Dudas, problemas técnicos y soluciones

Para centralizar las dudas o problemas sobre esta herramienta, así como para compartir
soluciones o sugerencias con todos los participantes del taller, haz uso de la siguiente discusión
en el repositorio de este taller:

[Foro técnico sobre Conda][foro]

## Más recursos útiles <a class="anchor" id="recursos"></a>

Esta web era sólo una guia introductoria. No es funcional documentarse o estudiar
mucho sin antes probar a instalar y usar la herramienta. Aprenderás de
manera más solida si con el uso te van surgiendo necesidades a las que vas
dando solución poco a poco. Puedes encontrar -o contribuir añadiendo- más información
útil en los siguientes listados.

### Documentación <a class="anchor" id="documentacion"></a>

Documentación oficial de la herramienta:

- [Conda][conda_docs]

### Tutoriales, Webinars y cursos gratuitos <a class="anchor" id="tutoriales"></a>

Otros tutoriales, webinars, videos de youtube y cursos gratuitos que puedes consultar:

- [Tutorial GeoHacweek](https://geohackweek.github.io/Introductory/01-conda-tutorial/)    
- [Tutorial MOLSSI](https://education.molssi.org/getting-started-computational-chemistry/05-anaconda/index.html)   
- [Capentries-incubator Conda for Data Scientists](https://carpentries-incubator.github.io/introduction-to-conda-for-data-scientists/)    
- [Kaust-VisLab Conda for Data Science](https://kaust-vislab.github.io/python-novice-gapminder/00-getting-started-with-conda/index.html)    




[anaconda]: https://www.anaconda.com/
[conda_docs]: https://docs.conda.io
[conda_user_guide]: https://docs.conda.io/projects/conda/en/stable/user-guide/index.html
[conda_forge]: https://conda-forge.org/
[miniconda]: https://docs.conda.io/en/latest/miniconda.html
[anaconda_conda_forge]: https://anaconda.org/conda-forge
[install_conda_linux]: https://docs.conda.io/projects/conda/en/stable/user-guide/install/linux.html
[install_conda_macOS]: https://docs.conda.io/projects/conda/en/stable/user-guide/install/macos.html
[install_conda_windows]: https://docs.conda.io/projects/conda/en/stable/user-guide/install/windows.html
[conda_getting_started]: https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html
[conda_cheat_sheets]: https://docs.conda.io/projects/conda/en/stable/user-guide/cheatsheet.html 
[foro]: https://github.com/uibcdf/Taller-Python/discussions/7

