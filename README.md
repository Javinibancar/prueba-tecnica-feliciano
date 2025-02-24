# prueba-tecnica-feliciano
Ibancar - Prueba técnica para Desarrollador Web

Instrucciones para Ejecutar Requisitos Previos Antes de empezar, asegúrate de que tu sistema tiene lo siguiente:

PHP 8.2 o superior: Verifica que PHP está instalado ejecutando php -v en tu terminal. 
Composer: Es una herramienta para gestionar dependencias en proyectos PHP. Si no lo tienes instalado, descárgalo desde su página oficial. 
MySQL: Asegúrate de tener un servidor de base de datos MySQL activo. 

Lo primero que debes hacer es clonar el repositorio donde está el proyecto.

Instalar Dependencias Una vez dentro del directorio del proyecto, instala las dependencias ejecutando el comando composer install. Esto descargará todas las librerías necesarias para que el proyecto funcione correctamente.

Configurar Variables de Entorno Copia el archivo de configuración predeterminado llamado .env.example y renómbralo a .env. Puedes hacerlo fácilmente con el comando cp .env.example .env. Luego, abre el archivo .env con tu editor de texto favorito y configura los datos de conexión a la base de datos. Asegúrate de modificar los siguientes campos:

DB_CONNECTION: Configúralo como "mysql". DB_HOST: Define la dirección del servidor de tu base de datos (por defecto es "127.0.0.1"). DB_PORT: Usa el puerto correspondiente (generalmente "3306"). DB_DATABASE: Especifica el nombre de tu base de datos. DB_USERNAME: Ingresa el nombre de usuario de tu base de datos. DB_PASSWORD: Proporciona la contraseña de tu usuario de la base de datos. 

Generar la Clave de Aplicación Laravel utiliza una clave de aplicación única para encriptar información. Genera esta clave ejecutando el comando php artisan key:generate.

Ejecutar Migraciones Ahora debes crear las tablas en tu base de datos. Para esto, ejecuta el comando php artisan migrate. Laravel tomará las migraciones definidas en el proyecto y las aplicará a tu base de datos.

Iniciar el Servidor Con todo listo, es hora de iniciar el servidor de desarrollo de Laravel. Hazlo ejecutando el comando php artisan serve. Esto pondrá el proyecto en marcha y te dará una URL, como http://127.0.0.1:8000. Copia esa URL y pégala en tu navegador para acceder al proyecto.

Ejecutar Pruebas Unitarias Si quieres verificar que todo funciona correctamente, puedes ejecutar las pruebas unitarias incluidas en el proyecto utilizando el comando php artisan test. Esto te dará información sobre el estado del proyecto y confirmará que todo está en orden.

