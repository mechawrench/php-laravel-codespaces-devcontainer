# PHP-Laravel-CodeSpaces-DevContainer

This repo provides the .devcontainer files needed to start a CodeSpace for Laravel on GitHub.

## Instructions
1. Copy .devcontainer folder to your project root
1. (Optional) Copy init_codespace.sh to project root
1. Push to repo
1. Access repo GitHub page, open in CodeSpaces
1. Container should build and IDE should open ready for use
1. (Optional) Run init_codespace.sh to create .env and run DB migrations/seeds
    ```bash
    . ./init_codespace.sh
    ```
## MariaDB access (ENV settings)
Please set your DB env variables to the following to use the MariaDB docker container
```env
DB_CONNECTION=mysql
DB_HOST=mariadb
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=secret
```

## Expose by BeyondCode
Expose is included with this build.  Expose allows you to share your site with others, see documentation at https://beyondco.de/docs/expose/introduction

To use Expose, simply run the command "expose"

## Notes
- CodeSpaces is currently in Closed Beta, you need access to use .devcontainer files
- Includes the following PHP extensions, you can add your own by adjusting the DOCKERFILE
    - bcmath mysqli pdo pdo_mysql zip
- To access your site you need to run the following:
    ```php
    php artisan serve
    ```

# Credits
https://github.com/PMessinezis/vscode.laravel.devcontainer/blob/master/Dockerfile
