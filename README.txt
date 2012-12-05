The archive htdocs.tgz contains the current version of wordpress with a few plugins that we are either planning on using or investigating already installed. It is also configured with multisite.

As far as our unique stuff goes, there is an additional file, _listener.php, which is the file that the installer will make requests to at some point. It is supposed to parse the data from the installer and add everything to the database in the proper format. For now, it just takes some sample data in a very generic format and adds it to a specific site's database. I also included a sample plugin with "POS Connect" pasted in a few places instead of the sample plugin's name. We can fix this up later when we have some actual settings and things like that to add.

1. Install apache/php/mysql
2. Enable mod-rewrite for apache
3. Extract the archive to your www or htdocs directory (wordpress should end up in /path/to/htdocs/)
4. Create a mysql user named 'posconnect' with the password 'abcdefg', or edit the wp-config.php file to use a mysql username and password of your choice
5. Create a database called posconnect and execute the queries provided in posconnect.sql
6. Log in to wordpress with the user 'admin' and password 'posconnect' to start messing around
