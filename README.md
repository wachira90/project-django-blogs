# project-django-blogs


## create database

````
CREATE DATABASE `myblogs` CHARACTER SET 'utf8' COLLATE 'utf8_general_ci';
````

## edit connection

````
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'myblogs',
        'USER':'root',
        'PASSWORD':'pass1234',
        'HOST': '172.16.1.5',
        'PORT': '3306',
    }
}
````

## set upload path 
````
STATIC_URL = '/static/'
MEDIA_URL = '/media/'
MEDIA_ROOT = os.path.join(BASE_DIR,'media/')
````