## Instalación


### Instalamos PyQt
Usamos Homebrew para esto:
```sh
brew install pyqt
```


## Empecemos a usar la librería

Creemos un archivo llamado `main.py` en el escritorio con el siguiente código:
```python
import sys
from PyQt4 import QtGui

def main():

    app = QtGui.QApplication(sys.argv)

    w = QtGui.QWidget()
    w.resize(250, 150)
    w.move(300, 300)
    w.setWindowTitle('Hello world!')
    w.show()

    sys.exit(app.exec_())


if __name__ == '__main__':
    main()
```

Nos movemos al escritorio o a donde lo hayas puesto con la terminal
```sh
cd ~/Desktop
```

Ejecutamos el código
```sh
python main.py
```

Debería aparecer una pequeña ventana :)