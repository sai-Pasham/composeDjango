# composeDjango


docker-compose run web django-admin.py startproject composeexample .

edit composeexample/settings.py
Replace the DATABASES = ... with the following:
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql',
         'NAME': 'postgres',
         'USER': 'postgres',
         'HOST': 'db',
         'PORT': 5432,
     }
 }
 
 
 docker-compose up
 
 http://localhost:8000/
 
 https://docs.docker.com/compose/django/#connect-the-database
