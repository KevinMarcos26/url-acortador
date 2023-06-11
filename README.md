# url-acortador

URL recortador flask
Web App Capaz de tomar un link y devolver una versión recortada

Construido con Flask

app

app 2

Ejecutar con Docker
Ejecutar sudo python3 run.py es todo lo que necesita

Captura de pantalla 2023-06-08 043052

Ejecutar
$ git clone https://github.com/KevinMarcos26/url-acortador
$ cd url_acortador-flask
$ pip install -r requirements.txt
$ flask run
Antes de Ejecutar**
Si intenta ejecutar el proyecto sin unos requerimientos necesarios previos, Lo mas probable es que obtengo errores.

Requerimientos (En orden de prioridad)
establecer variables de entorno
Entorno virtual
Dependencias
Crear base de datos
Ejecutar
Variables de entorno
$ export FLASK_APP=main.py
Estas son opcional, para hacer debug al código

$ export FLASK_DEBUG=1
$ export FLASK_ENV=development
Entorno virtual
Lo mas recomendable es ejecutar el proyecto en un entorno virtual con python3.9

Se recomienda usar virtualenv o venv

Desde el entorno virtual instalar las dependencias requeridas pip install -r requirements.txt

Crear base de datos
La base de datos debe ser creada con los siguiente comando

$ cd db
$ python init_db.py
No obtendrá ninguna salida

Sin embargo puede verificar su archivo en db/database.db

Importante
init_db.py Cada que se ejecuta verifica que no exista la base de datos database.db y si existe la ELIMINA, por ello debe ser ejecutado solo 1 vez

Ejecute
Ahora si, no debería obtener ningún error al ejecutar la app $ flask run

server on

Tests de pruebas
Para correr los Tests corra el siguiente comando desde la raíz del proyecto

  $ pre-commit run --all-files
