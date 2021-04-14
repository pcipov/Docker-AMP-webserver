# docker-webserver

Docker config files for AMP server (Apache+PHP+Mysql).
Just add this folder to your site's root folder, go inside it and run "docker-compose up -d".
Then open address "localhost" in webbrowser to show your web project, or "localhost:8080" to run phpmyadmin (be patient in waiting until mysql server creates all base mysql tables).
DB tables are located in subfolder "db". Docker will create it automatically.

You have to change hostname of mysql server to "db" in your project!

Folder structure:

- .docker
  - db
  - docker-compose.yml
  - Dockerfile

You can change config file docker-compose.yml:
 - Mysql version
 - Mysql root password
 - default Mysql charset and collation
 - phpmyadmin login name and password

You can change config file Dockerfile:
 - PHP version

To run docker commands, go to folder .docker.

Commands:

docker-compose up -d
 - downloads images, builds/rebuilds containers and starts servers

docker-compose up
 - the same as above one, but with console output

docker-compose down
 - stops all containers from docker-compose.yml

docker ps
 - shows running containers

docker ps -a
 - shows all containers
