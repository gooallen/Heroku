# Heroku



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
- pip freeze - requirements.txt (use the angle bracket after pip freeze. Youtube doesn't allow angle bracket in description :/ )
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
