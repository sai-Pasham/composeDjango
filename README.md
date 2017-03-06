# composeDjango


<code>docker-compose run web django-admin.py startproject composeexample .</code>

edit composeexample/settings.py
Replace the DATABASES = ... with the following:
</BR>
<code>
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql',
         'NAME': 'postgres',
         'USER': 'postgres',
         'HOST': 'db',
         'PORT': 5432,
     }
 }
</code> 
 
 <code>docker-compose up </code>
 
 http://localhost:8000/
 
 https://docs.docker.com/compose/django/#connect-the-database
