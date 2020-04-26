# Django-Docker-Starter

Create Project

```
docker-compose run web django-admin startproject mysite .
```

DON'T FORGET THE PERIOD

Connect DB

```
# setting.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'PASSWORD': 'postgres',
        'HOST': 'db',
        'PORT': 5432,
    }
}
```

```
docker-compose up
```

Add to .vscode/settings.json

```
  "files.associations": {
    "*.html": "django-html",
    "**/requirements{/**,*}.{txt,in}": "pip-requirements",
  },
```