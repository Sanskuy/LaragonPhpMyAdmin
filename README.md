# LaragonPhpMyAdmin
laragon-phpmyadmin
# LaragonPhpMyAdmin
laragon-phpmyadmin

you can also add/update phpMyAdmin easily yourself. Just download from its official site (https://www.phpmyadmin.net/downloads) and extract to {LARAGON_DIR}\etc\apps\phpMyAdmin. That's all.
Now, you can access phpMyAdmin at: http://localhost/phpmyadmin

=================================================================================
Note: After extracting, your folder will look like that:
C:\laragon\etc\apps\phpMyAdmin

=================================================================================
There is an alias in \etc\apache2\ which will point http://localhost/phpmyadmin to
{LARAGON_DIR}\etc\apps. The purpose of that is to separate your project data

=================================================================================
You can add phpMyAdmin easily yourself:
https://forum.laragon.org/topic/98/how-to-update-phpmyadmin

=================================================================================
First download the phpMyAdmin form here : https://www.phpmyadmin.net/downloads/
then extract the downloaded (rar,zip) to : {INSTALLATION_PATH}\laragon\etc\apps\rename the folder to phpMyAdmin
now go to http://localhost/phpmyadmin, and your there
=================================================================================
if you want to login to the phpMyAdmin you need to search in the phpmyadmin folder for a file called config.sample.inc and
duplicate it and rename it to config.inc open the file and search for : ~
$cfg['Servers'][$i]['AllowNoPassword'] = false;~
and set it to true : ~ $cfg['Servers'][$i]['AllowNoPassword'] = true;~
save the file and DONE you can login using username if : root
