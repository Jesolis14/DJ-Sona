# DJ-Sona

## Requerimientos
Para poder ejecutar este proyecto, es necesario contar de antemano con los siguientes programas:
* Python 3.12+
* pip 24.2+
* Makefile (opcional)

## Clonar proyecto
Para clonar el proyecto en tu computadora, ejecuta la siguiente línea de comando:
```bash
git clone https://github.com/Jesolis14/DJ-Sona.git
```

Para validar que el proyecto se haya clonado correctamente, ejecuta los siguientes comandos para verificar que tienes la última versión del proyecto:
```bash
cd DJ-Sona
git status
```

Si se cuenta con el programa `Makefile`. Para que el proyecto cuente con la estructura deseada, ejecuta el siguiente comando, el cual creará todas las carpetas necesarias para mantener organizada toda la información:
```bash
make init
```

## Crear un ambiente virtual
Para poder ejecutar el proyecto, utilizamos la opción nativa de Python `venv`. Primero, dirígete a la carpeta de tu proyecto.

Una opción es usar el comando `make` en la carpeta de nuestro proyecto para que lo cree automáticamente:
```bashrequirementsk
make create_environment
```

En caso de querer hacerlo manualmente, puedes crearlo con los siguientes comandos. Nosotros recomendamos crear este entorno en la carpeta del proyecto:
```bash
cd C:\ruta\tu\proyecto
python -m venv <NOMBRE_DEL_AMBIENTE>
```

Para activar nuestro entorno, usa el siguiente comando:
```bash
# Windows
.\NOMBRE_DEL_AMBIENTE\Scripts\activate

#Linux
source NOMBRE_DEL_AMBIENTE/bin/activate
```

Para desactivar el entorno virtual, utiliza el comando:
```bash
deactivate
```

## Instalar dependencias

Para instalar las dependencias necesarias, se pueden usar los comandos:
```bash
make requirements
```
O, en su defecto, hacerlo con:
```bash
pip install -r requirements.txt
```

## Comandos Make
Lista de comandos disponibles para el Makefile:
* `make create_environment`: Crea un entorno virtual e imprime el comando para activarlo.
* `make init`: Inicializa el proyecto y crea los archivos necesarios.

* `make requirements`: Instala las librerías necesarias del archivo `requirements.txt`.

* `make process`: Procesa los datos que haya en la carpeta `/data/raw` y guarda los resultados en `/data/processed`.