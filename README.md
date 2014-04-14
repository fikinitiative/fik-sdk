fik-sdk
=======

Fik Stores Development Tools

1. Create a database and a user with perms on it


2. Configure your hosts file (/etc/hosts):
127.0.1.1 fik-sdk.lc


3. Configure your virtualhost:
<VirtualHost *:80>
    ServerName fik-sdk.lc
    DocumentRoot "/path-to-fik-sdk/wp"
    <Directory "/path-to-fik-sdk/wp">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>

4. Don't forget restart apache!!!


5. Clone the fik-sdk:
git clone https://github.com/fikinitiative/fik-sdk.git /path-to-fik-sdk/


6. Edit wp-cli.local.yml file with your database and wordpress configuration.


7. Install fik-sdk:
cd /path-to-fik-sdk/
vendor/composer.phar self-update && vendor/composer install


Hooray!! Enjoy your fik-sdk installation on:
http://fik-sdk.lc

