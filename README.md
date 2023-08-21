# Django Template 
#### To create the project use:
`django-admin startproject --template <repo .zip url> <project_name> <directory>`
## How to run ?
#### chronologically
- create pipenv environment `pipenv install` then `pipenv shell`
- configure the pipenv interpreter 
  in **python interpreter** set **base interpreter** 
  as the path to your pipenv python3 executable
- generate django secret key using the `get_secret_key()` method in python console
- setup `.env` file based on `.env-default` file in the `env/` directory
- if db is setup run `python manage.py migrate` as the migrations are already prepared
- static files  `python manage.py collectstatic`
- finally `python manage.py runserver` to run the server