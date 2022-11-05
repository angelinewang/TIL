WHen you get off of `sqlite3`...

To connect to postgres database:

Inside `settings.py`, ensure that database user and password is added:
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'dbname',
        'USER': 'dbuser',
        'PASSWORD': PROD_DB_PASSWORD,
        'HOST': 'localhost',
        'PORT': '5432',
        }
    }
 ```
