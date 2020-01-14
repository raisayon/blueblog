# blueblog
blogging platform

#getting started
mkdir -p blueblog //anywhere you can setup
cd blueblog

virtualenv blue
cd blue (I used gitbash)
scripts/activate 

pip install django
django-admin.py startproject blueblog src

python manage.py migrate (In order to initialize the database file)

Documentation static files settings
https://docs.djangoproject.com/en/stable/howto/static-files/

INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
]
to setup templates
'DIRS': [os.path.join(BASE_DIR,'templates')],
