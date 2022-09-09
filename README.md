# INTRODUCCION
## Terminos Importantes:
# UNIT TEST(PRUEBAS UNITARIAS)
### Verifica que las unidades individuales de código funcionen según lo esperado.
# Feature Tests(Pruebas de Funcionamiento)
### Prueba de la forma en que las unidades individuales trabajan juntas y transmiten mensajes.
# Regression Tests(Pruebas Regresion)
### Describen exactamente lo que un usuario debería poder hacer.
# HTTP Test
### Permite hacer una solicitud http simple.
# Authenticating Responses(Autenticando Respuestas)
###Pruebas de aplicación en autenticación  y autorización.
# Database tests (pruebas de base de datos)
### Herramientas y afirmaciones para facilitar la prueba de aplicaciones basadas en bases de datos.
# Creando un Nuevo Proyecto en Laravel.
####Nos ubicamos en la carpeta xampp/htdocs/laravel2341240/ ; dentro de esta carpeta abrimos el cmd y ejecutamos el siguiente comando: laravel new (nombre del nuevo proyecto) ,en este caso es laravel new TestLaravel.
#### Despues en el mismo cmd ponemos el siguiente codigo code .  este se hace con el fin de abrir el proyecto que hemos acabado de crear directamente en el Visual Studio Code.
#### Nos ubicamos dentro de la raíz del proyecto laravel new TestLaravel , y nos encontramos la carpeta llamada tests(pruebas), si abrimos esta carpeta nos aparecerán dos subcarpetas, llamadas Feature (características) y Unit(unidades), y dos archivos php que es la aplicación de creación y la testcase.php.
# Ejecutando pruebas.
#### Nos ubicamos en la terminal y ejecutamos el siguiente comando: php artisan test, este se hace para ejecutan las pruebas que se encuentran en la carpeta Feature y Unit.


#### No se han realizado cambios en el proyecto y por esta razón los dos test nos salen PASS
#### Ejecutamos el siguiente comando: php artisan make:test  UserTest ,
##### Esto creara una nueva prueba dentro de la carpeta de  Feature (funciones,) llamado UserTest.php
#### Se vuelven ejecutar las pruebas de los test para verificar que el nuevo test creado funciona correctamente

#### hacemos un cambio en el archivo de UserTest, como sigue:
### Nos devuelve un error.

# Creación de pruebas unitarias (Creating Unit Tests)
#### En la terminal ejecutamos el siguiente comando php artisan make:test UserTest --unit, esto creara un archivo dentro de la carpeta de la unidad.
# Otros Ejercicios:
##### Ejecutamos el siguiente comando para crear una ui:
##### composer require laravel/ui

#### Con el comando php artisan ui react  - - auth se crea el módulo de autenticación y registro de usuarios que viene por defecto con laravel
##### npm install  y el comando npm run dev inicia el servidor de frontend
# Creando la base de datos en phpMyAdmin
##### Para este proyecto, se crea por phpMyAdmin con el nombre testlaravel
#### En el archivo .env se verifica que la base de datos tiene el mismo nombre que la que se acaba de crear.
##### por consiguiente seguimos con la migracion la cual ejecutamos con el siguiente comando php artisan migrate el cual crea las tablas. en phpMyAdmin
##### En el UserTest se modifica la función pública de test_login_form() y en la parte de Use se modifica Test\TestCase.y procedemos a ejecutar las pruebas en la terminal con el comando php artisan test.
##### Despues de hacer este paso nos deberia cargar todo PASS , pero al ejecutarla una de las pruebas sale que el test UserTest es FAIL, y si por ende queremos ejecutar en el navegador con el comando php artisan serve no saldra un error al querer ingresar en el Login.ejecuta el comando npm install suguiere una nueva version disponible,por lo que se ejecuta el comando sugerido  npm install -g npm@8.19.1 ,despues de este comando se lanza de nuevo el comando npm run dev, despues de hacer todo eso regresamos a la terminal ejecutamos el comando php artisan serve para abrir el navegador y por ende nos deberia cargar el login correctamente.el Error se soluciono cambiando en la parte del funcion 400  en lugar de 200 y todos los test van en PASS.

#### Se crea la aplicación para evitar que se creen dos usuarios con el mismo nombre o el mismo email, esta se crea en la parte de public function , entonces creamos dos arreglos  una llamada $user1 y  $user2 , se le ponen el 'name' y el 'email'. y en la parte de arriba nos deberia aparecer use App\Models\User .
##### Finalmente en la terminal ejecutamos el comando php artisan test , con el fin de verificar que la funcion PASS pase todas las pruebas.

![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen1.png?raw=true)

![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen10.png?raw=true)

![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen11.png?raw=true)
![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen12.png?raw=true)
![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen13.png?raw=true)
![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen14.png?raw=true)
![](https://github.com/Elysena/Test-Laravel/blob/master/img/Imagen16.png?raw=true)





