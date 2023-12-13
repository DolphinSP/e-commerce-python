# E-commerce_Python

# Pasos para dockerizar

1- Creación del fichero Dockerfile
2- Creación del fichero docker-compose.yml
3- Inicialización de los contenedores con las imagenes seleccionadasç
$ docker-compose run web django-admin startproject backend .
4- Poner los contenedores en funcionamiento
$ docker-compose up
5- Parar los contenedores
$ docker-compose down

# Para compilar el programa

1- Hacer un fork para su repositorio
2- Tener instalado el docker desktop
3- correr el comando
$ docker-compose build
4- Correr el contenedor docker
$ docker-compose up
5- Aceder a la url en el navegador
http://localhost:8000

6- Para crear una nueva app, se tiene que utilizar el comando
$ docker-compose run web python manage.py startapp "nombre de la app"

7- Para verificar que el programa está funcionando completamente, proba esta url
Debería de aparecer en su pantalla ("Hello Delphin Project")
$ http://localhost:8000/category/hello/

8- Se instaló una nueva dependencia, debe actualizar el requeriments.txt con el comando
$ docker-compose run web pip freeze > requirements.txt

9- Para correr a imagen, también puedes utilizar el comando
$ docker-compose build
$ docker up
