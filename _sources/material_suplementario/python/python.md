# Cómo instalar y trabajar con Python


## ¿Cómo se instala?

Por su popularidad y utilidad el interpretador de Python está seguramente
instalado en tu sistema operativo Linux o MacOS. No obstante compartimos a
continuación páginas web que te pueden ayudar a instalar Python en tu sistema
operativo.

### En Linux

- Instalación según [RealPython blog](https://realpython.com/installing-python/#linux)
- Instalación según [The Hitchhiker’s Guide to Python](https://docs.python-guide.org/starting/install3/linux/#install3-linux)

### En MacOS

- Instalación según [RealPython blog](https://realpython.com/installing-python/#macos-mac-os-x)
- Instalación según [The Hitchhiker’s Guide to Python](https://docs.python-guide.org/starting/install3/osx/)

### En Windows

Antes de comenzar a trabajar desde el Command Prompt (cmp) de Windows debes saber lo siguiente:

- es una aplicación de línea de comandos incluida en el sistema operativo Windows. 
- es una herramienta que permite al usuario interactuar con el sistema operativo mediante la introducción de comandos específicos en lugar de hacer clic en los iconos de la interfaz gráfica de usuario.
- puede ejecutar una gran variedad de comandos para realizar tareas en el sistema operativo, como crear y eliminar archivos y directorios, gestionar procesos y servicios, administrar redes, entre otras muchas opciones.
- se pueden realizar tareas complejas de manera más rápida y eficiente que con la interfaz gráfica de usuario de Windows. 

El Command Prompt se puede abrir desde el menú de inicio de Windows o presionando las teclas "Windows" + "R" y escribiendo "cmd" en el cuadro de diálogo "Ejecutar". 

#### ¿Cómo instalar Python en Windows?

Para instalar Python en Windows, sigue los siguientes pasos:

1. Descarga el instalador de Python desde el sitio web oficial de Python:
   https://www.python.org/downloads/windows/
2. Haz clic en la sección "Download", busca tu sistema operativo, en este caso
   Windows, y da clic.
3. Selecciona el instalador adecuado para tu versión de Windows (32 bits o 64
   bits). Si es el caso, selecciona la opción "Download Windows installer
  (64-bit)".
4. Una vez que se haya descargado el archivo, haz doble clic en él para abrir
   el instalador.
5. En la primera pantalla del instalador, asegúrate de que la opción "Add
   Python 3.x to PATH" esté seleccionada. Esto agregará Python al PATH del
   sistema, lo que te permitirá acceder a Python desde cualquier directorio en la
   línea de comandos.
6. Haz clic en "Install Now" para comenzar la instalación.
7. Espera a que se complete la instalación. Esto puede tardar unos minutos.
8. Una vez que se complete la instalación, puedes cerrar el instalador.
9. Para verificar que Python se haya instalado correctamente, abre la línea de
   comandos de Windows presionando la tecla de Windows + R, se abrirá el cuadro
   de diálogo "Ejecutar", escribe "cmd" y da Enter. 
10. Ingresar el comando que necesitas ejecutar en tu sistema, en este caso
    escribe "python" en la línea de comandos. Si se muestra el intérprete de
    Python, significa que Python se ha instalado correctamente.


- Instalación según [RealPython blog](https://realpython.com/installing-python/#windows)
- Instalación según [The Hitchhiker’s Guide to Python](https://docs.python-guide.org/starting/install3/win/)

## ¿Cómo se usa?

### En Linux

Para programar únicamente necesitamos un editor de texto. Y para ejecutar el
programa basta con tener el [interpretador o
compilador](https://blog.makeitreal.camp/lenguajes-compilados-e-interpretados/)
correspondiente al lenguaje que estamos usando.

Con el editor creamos un fichero de texto plano que contenga la secuencia de
órdenes a ejecutar, el programa. Por ejemplo, imagina que creas el fichero
'hola.txt' con la siguiente linea:

```python
print("hola!")
```

El interpretador lo puedes entender como el software que leerá tu texto y lo
ejecutará traduciéndolo, en ese mismo momento, a lenguaje máquina. En el caso
anterior, invocando el comando `python` y ofreciendole como argumento el
fichero 'hola.txt':

```bash
python hola.txt
```

Veremos que el resultado será la impresión en pantalla:

```
hola!
```

<div class="alert alert-info" role="alert">
<strong>Sugerencia:</strong> Para comenzar a aprender a programar en Python te sugerimos que despues de terminar esta unidad continues con la siguiente titulada <a href='../Programando/Programando.ipynb'>"Programando en Python"</a>
</div>

---

### En Windows

Hay varias formas de trabajar con Python en Windows. Algunas opciones son:

**Consola de Python**
Python viene con una consola integrada que puedes usar para
escribir código Python y ejecutarlo directamente en la consola. Para abrir la
consola de Python, haz clic en el botón de inicio, busca "Python" y selecciona
"Python 3.x.x" (donde "x.x" es la versión instalada). Esto abrirá la consola de
Python, donde puedes escribir código Python y ejecutarlo.

**Entornos de desarrollo integrado (IDE)**
Hay varios IDE disponibles para trabajar
con Python en Windows, como PyCharm, Visual Studio Code, Spyder, entre otros.
Estos IDE te proporcionan herramientas adicionales para escribir y depurar tu
código Python, y algunos incluyen integraciones con herramientas de control de
versiones como Git.

**Herramientas de línea de comandos**
En Windows, puedes usar la línea de comandos
para ejecutar scripts Python directamente desde la consola. Para hacer esto,
simplemente navega al directorio donde está almacenado el archivo Python usando
el comando "cd" y luego ejecuta el archivo usando el comando "python
nombre_del_archivo.py". Esto ejecutará el archivo Python y mostrará la salida
en la consola.

**Jupyter Notebook**
Jupyter Notebook es una aplicación web que te permite crear y
compartir documentos que contienen código Python, texto, visualizaciones y
otros elementos. Puedes instalar Jupyter Notebook en tu PC con Windows y usarlo
para escribir y ejecutar código Python en un entorno interactivo.

**JupyterLab**
JupyterLab es una evolución de Jupyter Notebook. Es un entorno
interactivo de desarrollo basado en la web para trabajar con notebooks, código
y datos. Proporciona una interfaz avanzada para crear, editar, ejecutar y
compartir notebooks Jupyter, que son documentos interactivos que contienen
código, texto explicativo, gráficos y otros elementos. Además, JupyterLab
también admite la edición de archivos de texto plano, la ejecución de
terminales de shell y la visualización de resultados de datos en una variedad
de formatos.

## Dudas, problemas técnicos y soluciones. <a class="anchor" id="dudas"></a>

Para centralizar esas dudas técnicas sobre el tema de este notebook o proponer
soluciones o sugerencias más técnicas que queremos encontrar en el futuro
comentadas y visibles para todos, haz uso del siguiente canal:

[Foro Técnico: Python](https://github.com/uibcdf/Academia/issues/5)

## Más recursos útiles <a class="anchor" id="recursos"></a>

El propósito de esta unidad es ser un documento únicamente introductorio.
Puedes encontrar -o contribuir añadiendo- más información útil en el siguiente
listado:

### Documentación <a class="anchor" id="documentacion"></a>
https://www.python.org/    
https://realpython.com/    
https://docs.python-guide.org/    
https://wiki.python.org/moin/SpanishLanguage    
http://www.scipy-lectures.org/intro/intro.html
https://github.com/damianavila/Python-Cientifico-HCC/blob/master/1_Python_Cientifico_Intro.ipynb    

### Tutoriales, Webinars y cursos gratuitos <a class="anchor" id="tutoriales"></a>
https://www.python.org/about/gettingstarted/    
https://docs.python.org/3/tutorial/    
http://docs.python.org.ar/tutorial/    
http://swcarpentry.github.io/python-novice-inflammation/   
https://www.datacamp.com/community/open-courses?tag=python
https://www.datacamp.com/community/tutorials?tag=python
https://realpython.com/tutorials/python/    
https://www.learnpython.org/    
https://www.datacamp.com/courses/intro-to-python-for-data-science    
https://docs.python-guide.org/intro/learning/    
https://www.codecademy.com/learn/learn-python    
https://pythonprogramming.net/   
http://www.scipy-lectures.org/
https://www.programiz.com/

