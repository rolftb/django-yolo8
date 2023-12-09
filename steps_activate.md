Claro, puedo ayudarte a generar un listado de requerimientos basado en los imports de tu código. Pero puedo mostrarte cómo hacerlo en Python usando el módulo pipreqs.

Primero, instala pipreqs si aún no lo has hecho. Puedes hacerlo ejecutando el siguiente comando en tu terminal:

```
pip install pipreqs
```

Luego, puedes generar el archivo de requerimientos ejecutando pipreqs en la carpeta de tu proyecto. Por ejemplo, si tu proyecto está en una carpeta llamada my_project, puedes ejecutar:

```
pipreqs my_project
```

Esto generará un archivo requirements.txt en la carpeta my_project que lista todas las bibliotecas importadas en los archivos Python de la carpeta y sus versiones actuales.

# AMBIENTE VIRTUAL

Para crear un nuevo entorno virtual para tu repositorio, puedes usar venv que es un módulo de Python para crear entornos virtuales. Aquí están los pasos:

1. Primero, navega a la carpeta de tu proyecto en la terminal. Por ejemplo, si tu proyecto está en una carpeta llamada my_project, puedes usar:
cd my_project

1. Luego, crea un nuevo entorno virtual en esa carpeta. Puedes llamarlo env o cualquier otro nombre que prefieras:
`python3 -m venv env`
1. Ahora, activa el entorno virtual. En Windows, usa:
`.\env\Scripts\activate`
En Unix o MacOS, usa:
`source env/bin/activate`

Finalmente, instala las dependencias de tu proyecto desde el archivo requirements.txt:

`pip install -r requirements.txt`


Esto instalará todas las bibliotecas listadas en tu archivo requirements.txt en el entorno virtual.


`pip install daphne `

`pip install opencv-python`

# activación del repositorio

## Creación de los datos sql

para construir el servidor sql se utilizó el comando 
`python manage.py migrate`

LUEGO DE REALIZAR UN MIGRATE:
python manage.py runserver

van a faltar folders por crear para ello se debe ejecutar el siguiente comando:
`python manage.py makemigrations` 

luego aún falta crear el folder `./media` y dentro de el `./media/json` utilizado para guardar el etiquetado

## se debe ejecutar 

`python manage.py runserver`

# Creación de super usuario

Esto es para poder acceder al panel de administración de django

`python manage.py createsuperuser`

(env) C:\Users\user\OneDrive\Documentos\Visual Solutions\Codigo\Artificial-Vision-Recognition-with-Django>python manage.py createsuperuser
Username (leave blank to use 'rolf'): 

Acá se debe ingresar el nombre de usuario, en este caso se ingresó rolf por default tras los : 
luego  se escribe el correo electrónico. rolf@vs.com
luego se debe ingresar la contraseña, en este caso se ingresó 123

para acceder al panel de administración se debe ingresar a la siguiente dirección:
http:// localhost:8000/admin

pero primero se debe ejecutar el servidor con el comando: `python manage.py runserver`
