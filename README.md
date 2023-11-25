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


To create the webserver , run the command <br>
> python manage.py runserver 

This would get the django webserver up and running in localhost:8000 . If you want to facilitate this in a different port , mention the port after the runserver keyword. 

