## Instalación


### Instalamos [MPMATH](https://github.com/fredrik-johansson/mpmath)
```sh
sudo python -m easy_install mpmath
```
Nos pedirá ingresar la contraseña de administrador.


### Instalamos [IPython](https://github.com/sympy/sympy)
```sh
pip install ipython
```


### Instalamos [SymPy](https://github.com/sympy/sympy)

Creamos una carpeta para nuestros repositorios, la pondremos en la raiz de nuestro usuario.
```sh
mkdir ~/repos; cd ~/repos
```

Clonamos el código fuente de SymPy:
```sh
git clone git://github.com/sympy/sympy.git
```

Vamos a la carpeta del código fuente:
```sh
cd sympy
```

Instalamos la librería:
```sh
sudo python setup.py install
```

Si quieres testear la instalación para ver si está correcta puedes correr:
```sh
./setup.py test
```

### Empecemos a usar la librería
Abrimos `ipython` en la terminal con:
```sh
ipython
```
Usemos el ejemplo que viene en la página de [SymPy](https://github.com/sympy/sympy):
```python
from sympy import Symbol, cos
x = Symbol('x')
e = 1/cos(x)
print e.series(x, 0, 10)
```

Para salir `ipython`, tanto como en cualquier otro entorno Python:
```python
exit()
```
