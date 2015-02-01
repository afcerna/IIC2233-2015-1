## Instalación


### Instalamos [pytest](http://pytest.org/latest/getting-started.html)
```sh
pytest pip install -U pytest
```
El argumento `-U` fuerza a que se actualicen los demás paquetes.


### Empecemos a usar la librería

Creemos un archivo `.py` para probar la librería. Este tendrá una función que recibe un número, le suma 1 y lo retorna.
También tendrá una función que falla una prueba y otra que la supera.

Le llamaremos `probando_pytest.py` y lo ubicaremos en el escritorio.

```python
# En creamos un archivo llamado probando_pytest.py en el escritorio con este código dentro

def func(x):
    return x + 1

def test_answer_good(): # Hagamos una prueba satisfactoria
	assert func(3) == 4

def test_answer_bad(): # Hagamos que falle a proposito
    assert func(3) == 5
```

Nos movemos al escritorio o a donde lo hayas puesto con la terminal
```sh
cd ~/Desktop
```

Ejecutamos las pruebas
```sh
py.test probando_pytest.py
```
Debería decirnos que hay un error en la función `test_answer_bad`
