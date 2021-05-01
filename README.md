#  Mychat
## _Setting up chatrooms using BLAB AX_

[![N|Solid](https://justblab.com/img/bws_screen.png)](https://justblab.com/blabax-php-ajax-website-chat-software)

## Requirements
Any Linux / Windows host or shared hosting service with PHP/MySQL and PHP mysqli extension enabled
If you are still running PHP5: PHP json extension enabled (bundled with PHP7+)
Optional: PHP fileinfo & GD extensions enabled in order to recognize file types and resize uploaded avatars
How to install
Download BlaB! AX at the bottom of this page and unzip the files in an empty folder e.g. /mychat
Upload the folder /mychat to your server with an FTP program and CHMOD config.php to 666 and /attachments to 777.
Navigate with your browser to YOUR-URL.COM/mychat/ - the install will start automatically:
Step 1: submit MySQL host, user, password and database name.
Step 2: create your admin account (username, password, email etc)
That's all!

## DataBase config
- ssh into MySql container or use phpMyAdmin to create a database and a user

## Config
- delete blabax/config.php file
- add/modify settings in /blabax/install/phpconfig match with the MySql config
- first time running will require installing: http://localhost:8080/install


## Tech

- [PHP] 
- [Docker]
- [Docker-Compose] 
- [MySql]

## Runing the cluster

```sh
cd mychat
docker-compose up
```

Server runs at http://localhost:8080