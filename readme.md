## WP manual migration steps

* 1. Transfer files
* 2. Transfer database
* 3. Connect database + wp
* 4. Change website URL


## Transfer files

* Then create a zip file of Wp site from localhost.
* Upload the zip file to public_html folder of live server.


## Transfer database

* First of all create a dbName, userName, pass to cPanel. For example dbName= new_db, userName= new_user, pass= 123456
* Export the existing db from localhost/otherServer phpmyadmin. It will download to pc as xyz.sql file. 
* Import the downloaded file to new db.


## Connect DB+ WP

*  After completed two steps, go to "wp-config.php" file from live server directory. Then edit the dbName, userName and password as new_db, new_user and 123456.


## Change website URL

* Now go to db (new_db) from live server. There have a table as "wp-options". Open it then edid 2 rows value (siteurl, home). For example siteurl= https://www.timeshub.com and home= https://www.timeshub.com
