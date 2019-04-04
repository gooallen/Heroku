# Heroku


## Django
https://devcenter.heroku.com/articles/django-app-configuration

- Copy the project seperately
- Go to 'Getting Started on Heroku with Python'
- Create an Heroku account
- install pipenv
- Install git ( check git --version)
- Install Heroku CLI
- Login heroku
```
heroku login
```
- Create a virtual enviroment
- Run manage.py not gonna run - pip freeze nothing installing
- Check which version django,requests you have and install it
- Run manage.py and then stop it
- Go to django heroku
- Create a Procfile
```
** The location of setting is important, For example setting is under 'mytasks' folder, it should be like below
web: gunicorn mytasks.wsgi

** latest version
web: gunicorn fundraisingproject.wsgi
```
- Install django-heroku
- Add stuff to settings.py file
```python
import django_heroku
# ..
# Activate Django-Heroku.
django_heroku.settings(locals()) # in the end
```
- Install guincorn 
- pip freeze > requirements.txt
- Create 'requirements.txt' (pip freeze available)
```
dj-database-url==0.5.0
Django==2.1.7
django-heroku==0.3.1
gunicorn==19.9.0
psycopg2==2.7.7
pytz==2018.9
whitenoise==4.1.2
```
- heroku create <project name> (to create an app on heroku)
- git status git commands - (git push heroku master
```
git init
git status
git add --all
git commit -m "name"
heroku git:remote -a <project name>
git push heroku master
```
- Open up the website)
- Admin panel not working. heroku run bash. Migrations
```
heroku run bash
# ..
python manage.py migrate
python manage.py createsuperuser

```
  
  
