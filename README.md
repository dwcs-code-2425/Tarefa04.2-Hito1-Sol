# Comandos ejecutados
composer require symfony/security-bundle
php bin/console make:user 
php bin/console doctrine:database:create

php bin/console make:migration  

php bin/console doctrine:migrations:migrate


composer require symfonycasts/verify-email-bundle
php bin/console make:registration-form


php bin/console make:security:form-login