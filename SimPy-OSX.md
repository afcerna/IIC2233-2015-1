## Instalación

### Instalamos [MPMATH](https://github.com/fredrik-johansson/mpmath)
```
sudo python -m easy_install mpmath
```
Nos pedirá ingresar la contraseña de administrador.



Creamos una carpeta para nuestros repositorios, la pondremos en la raiz de nuestro usuario:
mkdir ~/repos2; cd ~/repos2

Clonamos el código fuente de SymPy:
git clone git://github.com/sympy/sympy.git

Vamos a la carpeta del código fuente:
cd sympy

Instalamos la librería:
sudo python setup.py install