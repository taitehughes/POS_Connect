The archive wptest.tgz contains the current version of wordpress with a few plugins that we are either planning on using or investigating already installed. It is also configured with multisite. Steps to get set up are included below.

1. Install apache/php/mysql
2. Enable mod-rewrite for apache
3. Extract the archive to your www or htdocs directory (wordpress should end up in /path/to/www/wptest)
4. Create a mysql user named 'wptest' with the password 'abcdefg', or edit the wp-config.php file to use a mysql username and password of your choice
5. Create a database called wptest and execute the queries provided in wptest.sql
6. Log in to wordpress with the user 'admin' and password 'wptest' to start messing around
