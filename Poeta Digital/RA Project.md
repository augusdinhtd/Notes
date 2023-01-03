su-------**Account**---------
URL QC: 
	- Client: https://realauth.poeta-internal.com/
	- Admin: https://realauth.poeta-internal.com/ra-auth-admin-1/sign-in

URL Prod:
	- https://app.realauthentication.com/sign-in
	khoa+client@poetadigital.com
	Abcd1234@

Account:
	- Admin:
		admin@admin.com
		!RealAuth2019
		
	- Authenticator:
		khoa+reviewerc@poetadigital.com
		@Abcd1234
		
		khoa+reviewerd@poetadigital.com
		Abcd1234@
		
	- Customer:
		Business:
			khoa+business@poetadigital.com
			Abcd1234@
			dinhtd9@gmail.com
		   Abcd@1234
		Individual:
			khoa@poetadigital.com
			Abcd1234@

---------To Read--------
Component UI sử dụng với Stitches: https://www.radix-ui.com/

---------Set up envirnoment--------
Run project:
1. Open CMD window: bash
2. Check ip a
3. Open window+R drivers (etc/hosts)
4. Change file /etc/hosts
5. sudo service apache2 start
6. sudo /etc/init.d/mysql start
7. sudo service elasticsearch start
8. If code change: cd ./www/front npm run build:main or yarn build:main

1: add the PPA maintained by Ondrej Surýsudo add-apt-repository ppa:ondrej/php  
2: update the systemsudo apt update  
3: install PHP versions 7.2sudo apt install php7.2  
4: Select the standard version of PHP  
sudo update-alternatives --config php  
or  
sudo update-alternatives --set php /usr/bin/php7.2  
5: Disable version 7.4 or the one you are usingsudo a2dismod php7.4  
6: enable version 7.2sudo a2enmod php7.2  
7: Restart the apache serversudo systemctl restart apache2

sudo apt install php7.3-common php7.3-mysql php7.3-xml php7.3-xmlrpc php7.3-curl php7.3-gd php7.3-imagick php7.3-cli php7.3-dev php7.3-imap php7.3-mbstring php7.3-opcache php7.3-soap php7.3-zip php7.3-intl -y

php artisan route:list (edited)

composer install  
[http://realauth-api.local](http://realauth-api.local/)  
cd /etc/apache2/sites-available/  
sudo xdg-open 000-default.conf  
sudo xdg-open /etc/hosts  
at www folder: sudo chmod -R 777 storage/*  
sudo service apache2 restart`sudo apt update`  
`sudo apt install php7.4`  
`sudo apt install php7.4-common php7.4-mysql php7.4-xml php7.4-xmlrpc php7.4-curl php7.4-gd php7.4-imagick php7.4-cli php7.4-dev php7.4-imap php7.4-mbstring php7.4-opcache php7.4-soap php7.4-zip php7.4-intl -y`  
`npm run dev`  

sudo a2enmod rewrite
sudo service apache2 restart

<VirtualHost *:80>  
    # The ServerName directive sets the request scheme, hostname and port that  
    # the server uses to identify itself. This is used when creating  
    # redirection URLs. In the context of virtual hosts, the ServerName  
    # specifies what hostname must appear in the request's Host: header to  
    # match this virtual host. For the default virtual host (this file) this  
    # value is not decisive as it is used as a last resort host regardless.  
    # However, you must set it for any further virtual host explicitly.  
    ServerName realauth-api.local    #ServerAdmin webmaster@localhost  
    DocumentRoot /var/www/html/BFS_RLA/www/public/ # Available loglevels: trace8, ..., trace1, debug, info, notice, warn,  
# error, crit, alert, emerg.  
# It is also possible to configure the loglevel for particular  
# modules, e.g.  
#LogLevel info ssl:warn ErrorLog ${APACHE_LOG_DIR}/error.log  
CustomLog ${APACHE_LOG_DIR}/access.log combined # For most configuration files from conf-available/, which are  
    # enabled or disabled at a global level, it is possible to  
    # include a line for only one particular virtual host. For example the  
    # following line enables the CGI configuration for this host only  
    # after it has been globally disabled with "a2disconf".  
    #Include conf-available/serve-cgi-bin.conf  
    <Directory "/var/www/html/BFS_RLA/www/public/">  
        AllowOverride All  
    </Directory>  
</VirtualHost># vim: syntax=apache ts=4 sw=4 sts=4 sr noet

dinhtran@Poeta-TDDinh:/mnt/c/Users/Poeta$ cd /etc/
dinhtran@Poeta-TDDinh:/etc$ cd apache2/sites-enabled/
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ ls
ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ ls ..
apache2.conf    conf-enabled  magic           mods-enabled  sites-available
conf-available  envvars       mods-available  ports.conf    sites-enabled
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ cd ..
dinhtran@Poeta-TDDinh:/etc/apache2$ cd sites-available/
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$ nano ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$ cd ..
dinhtran@Poeta-TDDinh:/etc/apache2$ nano apache2.conf
dinhtran@Poeta-TDDinh:/etc/apache2$ nano apache2.conf
dinhtran@Poeta-TDDinh:/etc/apache2$ cd sites-enabled/
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ ls
ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ cd ra.conf
-bash: cd: ra.conf: Not a directory
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ nano ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ cd ,,
-bash: cd: ,,: No such file or directory
dinhtran@Poeta-TDDinh:/etc/apache2/sites-enabled$ cd ..
dinhtran@Poeta-TDDinh:/etc/apache2$ cd sites-available/
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$ ls
000-default.conf  default-ssl.conf  ra.conf  ra.conf.save
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$ nano ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$ nano ra.conf
dinhtran@Poeta-TDDinh:/etc/apache2/sites-available$

--------------------------------------------
Nếu thêm mới icon thì chạy lệnh này trước khi commit code
npx svgo www/front/icons/sort-asc.svg

------------------------------------------------------
Migrate
dinhtran@Poeta-TDDinh:/mnt/d/2.Project/BFS_RLA/www$ php artisan migrate

Migrating: 2022_11_17_030828_add_new_setting_add_permission_final_order
Migrated:  2022_11_17_030828_add_new_setting_add_permission_final_order (0.06 seconds)
dinhtran@Poeta-TDDinh:/mnt/d/2.Project/BFS_RLA/www$

-------------------------------------------
Git
git reset --hard HEAD