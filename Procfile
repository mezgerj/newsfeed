release: python manage.py migrate
web: gunicorn config.wsgi:application
worker: celery worker --app=newsfeed.taskapp --loglevel=info
