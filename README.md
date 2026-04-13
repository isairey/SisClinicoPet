# Pet Care (Sistema de Gestión de Pacientes)

Este es un sistema básico de gestión de pacientes diseñado específicamente para veterinarios. 

La aplicación está construida utilizando Laravel, Inertia y Vue 3 con un enfoque basado en API, proporcionando una experiencia de usuario fluida.

# Características
La aplicación permite a los veterinarios gestionar:

- Clientes: Mantén un registro de todos tus clientes en un solo lugar. Agrega, actualiza y elimina la información de los clientes según sea necesario.
- Pacientes: Gestiona toda la información de los pacientes, incluyendo historial médico, planes de tratamiento y más.
- Citas: Programa y gestiona citas. El sistema permite ver tu calendario.
- Inventario: Lleva el control de todo el inventario de tu clínica. Esto incluye medicamentos, equipo y cualquier otro artículo necesario para tu práctica.

# Instalación

Instalar dependencias de PHP

composer install

Generar una nueva clave de la aplicación

php artisan key:generate

Vincular el directorio de imágenes

php artisan storage:link

Instalar paquetes de Node

npm install

Migrar la base de datos

php artisan migrate

Poblar las tablas `species` y `breeds`
```
php artisan db:seed --class=SpeciesSeeder

php artisan db:seed --class=BreedsSeeder
```

# Pruebas
Probar el `ClientController`

./vendor/bin/phpunit tests/Feature/ClientTest.php


# Seeders
Para desarrollo local

php artisan db:seed --class=UserSeeder

php artisan db:seed --class=ClientsSeeder

php artisan db:seed --class=SpeciesSeeder

php artisan db:seed --class=BreedsSeeder

php artisan db:seed --class=PetsSeeder

php artisan db:seed --class=ItemsSeeder


# Capturas de Pantalla

![Tabla de mascotas](https://i.imgur.com/GAqDR3K.png)

![Editar Mascota](https://i.imgur.com/s0aeu2Q.jpeg)

![Calendario](https://i.imgur.com/H1uGqa3.jpeg)
```
