# Comandos ejecutados

1. Se creó el proyecto 
composer create-project symfony/skeleton:"7.2.x" tarea0421 

2. Se añadieron las dependencias para una webapp 
cd tarea0421
composer require webapp


3. Se editó .env para añadir la cadena de conexión a la BD. Se creó la base de datos: php bin/console doctrine:database:create

4. Se creó el controlador
 php bin/console make:controller Hello 

Se ejecutaron los pasos de la documentación: 
5. composer require symfony/security-bundle
6. php bin/console make:user
7. php bin/console make:migration
8. php bin/console doctrine:migrations:migrate
9. composer require symfonycasts/verify-email-bundle
10. php bin/console make:registration-form
11. php bin/console make:security:form-login

12. Para redirigir a /hello, se cambió el fichero security.yaml para añadir 
default_target_path bajo form_login
Esto se puede ver en la documentación oficial: https://symfony.com/doc/current/reference/configuration/security.html#default-target-path