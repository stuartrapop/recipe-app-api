# recipe-app-api

Recipe Api

run all commands through docker compose
docker-compose run --rm app sh -c "python manage.py connectstatic"

#lint files
docker compose run --rm app sh -c "flake8"

#create django project via docker ?? a bit strange
docker compose run --rm app sh -c "django-admin startproject app ."

#create super users
docker compose run --rm app sh -c "python manage.py createsuperuser"

#create a new project within the app
docker compose run --rm app sh -c "python manage.py startapp recipe"

#docker up
docker compose up
