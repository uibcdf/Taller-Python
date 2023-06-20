# Reto semanal

Esta segunda semana tienes que resolver unas tareas cuyo objetivo es estar
seguros de que la semana próxima tienes el entorno adecuado para poder comenzar
a programar en Python. Son las siguientes:

## Crea un entorno de trabajo en Conda

Instala Conda, si no lo has hecho ya, y crea un entorno de trabajo para el taller con Python 3.10.
Por ejemplo, con el nombre "Taller-Python":

```bash
conda create -n Taller-Python python=3.10
```

Actívalo para instalar lo necesario y resolver el resto de secciones del reto:

```bash
conda activate Taller-Python
```

## Abre el interpretador Python

Si hiciste la sección anterior y estás con tu entorno "Taller-Python" activo.
Abre Python y prueba a ejecutar:

```python
print('Hola mundo!')
```

## Escribe un script en Python

Escribe un script de Python cuya función sea imprimir en pantalla un texto.
Dáselo a Python para que lo ejecute. Y cuando creas que tu script funciona correctamente,
súbelo a tu fork del taller para compartirlo con nosotros
(ubícalo en este mismo directorio).

## Instala iPython

Instala iPython 3.10.

Con el entorno activado:
```bash
conda install ipython
```

Ábrelo y prueba a ejecutar:

```python
print('Hola mundo!')
```

¿Qué diferencias ves con el interpretador de Python original?

## Instala Jupyter Lab

Instala Jupyter Lab con Python 3.10.

Con el entorno activado:
```bash
conda install jupyterlab
```

Ábrelo y crea un Jupyter Notebook con
kernel de Python. En él, edita dos celdas.
La primera celda será de texto en Markdown:

```markdown
# Saludo al mundo desde Google Colab
```

La segunda será de código en Python:

```python
print('Hola mundo!')
```

Guarda el notebook y súbelo a tu fork del taller para compartirlo con nosotros
(colócalo en este mismo directorio).

## Abre una sesión en Google Colab

Abre una sesión en Google Colab y crea un Jupyter Notebook. En él, edita dos celdas.
La primera celda será de texto en Markdown:

```markdown
# Saludo al mundo desde Google Colab
```

La segunda será de código en Python:

```python
print('Hola mundo!')
```

Ejecuta ambas celdas y descarga tu notebook. Al igual que hiciste en la sección
anterior, sube este notebook a tu fork para compartirlo con nosotros.

## Ya puedes desactivar el entorno de Conda

Ya puedes desactivar el entorno de Conda 'Taller-Python':

```bash
conda deactivate
```

