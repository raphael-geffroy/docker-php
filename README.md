# docker-php

This is my Docker stack for php development
It contains a php service with : php-fpm(listening 9000), composer and symfony cli
a nginx service watching /srv/app/public(/index.php)
Optionnaly you can add a Database service

To use it:

- add a .env file with GIT_EMAIL & GIT_USER_NAME

If you want to create a symfony project :

- ssh to the php service
- $cd /srv
- $symfony new app

If you want to create a Vanilla php project :

- just add a public directory inside app
- create a index.php inside it
