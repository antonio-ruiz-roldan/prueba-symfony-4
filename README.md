# prueba-symfony-4
Prueba de Symfony 4: Login y Registro de Usuarios con acceso a Asignaturas y Cursos

Para lanzar la aplicación:
php -S 127.0.0.1:8000 -t public

Necesario el uso de la libreria Markebundle 
composer require symfony/maker-bundle --dev

Creación clase User (Necesario composer require orm)
php bin/console make:user 
php bin/console doctrine:generate:entities User


Creación formulario de Login (Necesario composer require security // composer require twig)
php bin/console make:auth 

Creación formulario de Registro (Necesario composer require form validator)
php bin/console make:registration-form

Creación de Cursos (Necesario composer require annotations, aplicable tambien a Asignaturas (por hacer))
php bin/console make:entity Courses
php bin/console make:crud Courses

Para los cambios de archivos twig y css
composer require symfony/asset
