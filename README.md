# PHP-Laravel-CodeSpaces-DevContainer

This repo provides the .devcontainer files needed to start a CodeSpace for Laravel on GitHub.

## Instructions
1. Copy .devcontainer folder to your project root
1. (Optional) Copy init_codespace.sh to project root
1. Push to repo
1. Access repo GitHub page, open in CodeSpaces
1. Container should build and IDE should open ready for use

## Notes
- CodeSpaces is currently in Closed Beta, you need access to use .devcontainer files
- To access your site you need to run the following:
    ```php
    php artisan serve
    ```

# Credits
https://github.com/PMessinezis/vscode.laravel.devcontainer/blob/master/Dockerfile