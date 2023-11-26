# djangoweb

Advantages:

1. The admin site
2. Object relational mapper
3. authentication
4. caching

**Client** generates the web page and **server** delivers the data required for the webpage. The **server** would be able to serve many clients and also different endpoints data could be configured in the server side. 

Server provides an interface that could be used by the clients to connect to these endpoints , which is called **API** 


First django project:

mkdir storefront

cd storefront/

pipenv install django

pip install django

ls -lrt

pip install pipenv

pipenv install django


To activate the virtual environment and use the python interpreter inside the virtual environment and not to use the global interpreter. <br>
_> pipenv shell _

Using django-admin , create the project <br>
_> django-admin startproject <projectname> ._ 

**Creation of APP**

> python manage.py startapp <appname> 

Once the app is created then, it must be referenced in the settings.py under the installed apps section

**Create Migrations**


Once the models.py are created based on the requirement inside each app. The migrations could be created. 
To create a migration . Run 

_> python manage.py makemigrations_

If you want to make any changes in the data within the models, then the makemigrations must be again run. 

Once complete we can run the migrate command

_> python manage.py migrate_

_Note:_ _Add the mysqlite extensions. Go-To Command Pallette -> SQL: Add Database_

You would be able to see a similar screen in the VSCODE explorer section.
<img width="729" alt="image" src="https://github.com/sunilharipkd/djangoweb/assets/111420932/65b64a65-b4da-476b-937a-8229be8f7d42">

**Undo changes in Database**
If you want to make a specific change within a migration, you can edit the class contents and then run the migrate .
But if you want to revert the last migration , then you can run the migrate against a specific migration number. 
For EX: 

<img width="174" alt="image" src="https://github.com/sunilharipkd/djangoweb/assets/111420932/ac56ac51-3176-4056-b14a-9857b492223b">

I have 4 migration files, and if I want to revert the last changes that has gone in 004 , then we can get this done by 
> python manage.py migrate storeapp 003

Note: Post this , the code changes need to be reverted. Either use the git versioning to revert changes or do it manually.

**Only by doing this the revert operation is complete. **


To create the webserver , run the command <br>
> python manage.py runserver 

This would get the django webserver up and running in localhost:8000 . If you want to facilitate this in a different port , mention the port after the runserver keyword. 

