python -m django-admin startproject name

Django project consists of 
asgi.py
settings.py
urls.py
wsgi.py

python manage.py startapp name

Django app consists of 

migrations
init.py
admin.py
apps.py
urls.py
views.py
models.py
tests.py

python manage.py runserver

to make view work, bind it to a url -> urls.py -> urlpatterns["", views.index, name="index"]

register app in project urls.py


To create admin panel
python mange.py createsuperuser
Register model in admin.py in polls app, it will be displayed in admin panel.

return render(request, views.index, name='index'')



Deploying django application
1. Dedicated servers, expensive
2. Containerization and Orchestration using kubernetes and docker-compose
3. Serverless using AWS lambda, Azure functions or Google cloud fucntions
4. Traditional Web hosting using web server apache or nginx and wsgi server gunicorn.
5. Virtual Private Server (VPS) - Linode, server will be provided by them.


Django performance optimization
1. Database optimization - Stored procedures, indexing, database sharding, storing frequently used query in cache.
2. Static files optimization - using cdn or amazon s3 to store static files related to your django app
3. Asynchronous processing - offload long running tasks to background
4. load balancing
5. django middlewares and setting - disable unneccessary middlewares