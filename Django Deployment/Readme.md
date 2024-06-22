##### Create an EC2 instance

```
ssh -i "<file>.pem" ubuntu@[public dns]
```
```
sudo su
```
```
apt intall apache2
```
```
ufw app info "Apache Full"
```
```
ufw allow in "Apache Full"
```
```
apt install python3-pip
```
```
apt install libapache2-mod-wsgi-py3
```
```
cd /var/www/
```
```
mkdir <project>
```
```
cd <project>
```
```
apt install python3-virtualenv
```
```
virtualenv prodenv
```
```
source prodenv/bin/activate
```
```
pip install Django
```
```
django-admin startproject demo
```


###### add into settings.py
```
import os
```
```
STATIC_ROOT = os.path.join(BASE_DIR, 'static/')
```

```
python manage.py makemigrations
python manage.py migrate
python manage.py collectstatic
```
```
python manage.py runserver
```
```
python manage.py createsuperuser
```

```
cd /etc/apache2/sites-available/
vim 000-default.conf
```

###### comment the document root

##### add following configuration to file

```
Alias /static "path to project"/static
        <Directory /var/www/chgproject/demo/static>
           Require all granted
        </Directory>

        <Directory /var/www/chgproject/demo/demo>
                <Files wsgi.py>
                    Require all granted
                </Files>
        </Directory>

        WSGIDaemonProcess chgproject python-path=/var/www/chgproject/demo python-home=/var/www/chgproject/prodenv
        WSGIProcessGroup chgproject
        WSGIScriptAlias / /var/www/chgproject/demo/demo/wsgi.py

```
```
a2dissite 000-default.conf
```

```
a2ensite 000-default.conf
```

```
service apache2 restart
```
