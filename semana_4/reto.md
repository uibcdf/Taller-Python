# Reto semanal

## Implementación de tu primera librería

Como reto semanal debes implementar tu propia librería con las siguientes características:

- La librería debe contener al menos una función.
- La librería debe contener al menos una clase con al menos un método y un atributo.

Puedes llamar a la librería con el nombre que quieras, supongamos que se llama 'Tamagochi'. Deberás
crear en el directorio 'semana\_4' de tu clon local el directorio llamado 'tamagochi'. Como ves, la
sugerencia es que el nombre de la librería que vas a usar sea en letras minúsculas y sin espacios
(puedes usar guiones bajos pero se desaconseja).

### Estructura de la librería

Vamos a suponer que vas a escribir tu función llamada 'saludo' en el fichero 'funciones.py'. Y tu
clase llamada 'Atomo' en el fichero llamado 'atomo.py'. Esta es la estructura que deberá tener tu
librería:

```bash
tamagochi
        |
        |- __init__.py
        |- funciones.py
        |- atomo.py
```

#### Fichero 'funciones.py'

Escribamos en este fichero la definición de la función:

```python
def saludo(argumento_1, argumento_2, ...):

    # Definición de la función

    return output
```

#### Fichero 'atomo.py'

Escribamos en este fichero la definición de la clase con al menos un atributo y un método:

```python
class Atomo():

    # Definición de la función

    def __init__(self, primer_color):

        self.color = primer_color

        # definición de __init__

    def cambio_color(self, nuevo_color):

        self.color = nuevo_color

```

#### Fichero '__init__.py'

El fichero '__init__.py' organiza el primer nivel de la librería. Podemos por ejemplo dale la
siguiente estructura:

```python
from .atomo import Atomo
from .funciones import saludo
```


### Empuja tu librería a tu fork en GiHub

Prueba que tu librería puede ser importada cuando Python se abre en el mismo directorio 'semana_4'.
Empuja tu librería a tu clon remoto de tu fork en GitHub para compartir con los participantes del
taller y sus tutores tu resolución del reto.
