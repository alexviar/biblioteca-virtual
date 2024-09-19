# Biblioteca Virtual de Trabajos de Grado

Este proyecto es una biblioteca virtual que permite a los usuarios acceder a tesis, monografías y proyectos de fin de carrera. Está desarrollado en Laravel y permite a los estudiantes y profesores buscar, descargar y subir trabajos académicos de forma organizada.

## Tabla de Contenidos

- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Características](#características)
- [Contribuir](#contribuir)
- [Licencia](#licencia)

## Requisitos

Antes de instalar el proyecto, asegúrate de tener lo siguiente:

- PHP >= 8.0
- Composer
- MySQL o cualquier otra base de datos compatible
- Node.js y NPM (para la compilación de assets front-end)

## Instalación

Sigue los siguientes pasos para instalar el proyecto:

1. Clona el repositorio:

    bash
    git clone https://github.com/usuario/biblioteca-virtual-trabajos-grado.git
    

2. Accede al directorio del proyecto:

    bash
    cd biblioteca-virtual-trabajos-grado
    

3. Instala las dependencias de PHP con Composer:

    bash
    composer install
    

4. Instala las dependencias de Node.js:

    bash
    npm install
    

5. Crea el archivo .env y configura tu base de datos y otras variables de entorno:

    bash
    cp .env.example .env
    

6. Genera la clave de la aplicación:

    bash
    php artisan key:generate
    

7. Ejecuta las migraciones para crear las tablas en la base de datos:

    bash
    php artisan migrate
    

8. Opcional: Si quieres poblar la base de datos con datos de ejemplo, puedes ejecutar el seeder:

    bash
    php artisan db:seed
    

9. Compila los assets front-end:

    bash
    npm run dev
    

10. Inicia el servidor de desarrollo:

    bash
    php artisan serve
    

Accede a la aplicación en [http://localhost:8000](http://localhost:8000).

## Uso

Una vez que la aplicación esté en funcionamiento, los usuarios podrán:

- Buscar trabajos de grado por título, autor o categoría.
- Visualizar detalles de los trabajos y descargar archivos en PDF.
- Subir nuevos trabajos de grado (solo para usuarios autenticados).

## Características

- *Búsqueda avanzada:* Permite filtrar trabajos por palabras clave, autor o año de publicación.
- *Sistema de roles y permisos:* Solo los administradores pueden aprobar o rechazar trabajos subidos.
- *Gestión de usuarios:* Registro e inicio de sesión para estudiantes y profesores.
- *Interfaz de usuario moderna:* Construida con Laravel Blade y Tailwind CSS.

## Contribuir

¡Las contribuciones son bienvenidas! Si deseas contribuir, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama (git checkout -b feature/nueva-funcionalidad).
3. Realiza tus cambios y haz commit (git commit -m 'Agrega una nueva funcionalidad').
4. Haz push a la rama (git push origin feature/nueva-funcionalidad).
5. Abre un pull request.

Por favor, asegúrate de que tus cambios no rompan la funcionalidad existente y de que sigan las convenciones de código de Laravel.

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más información.