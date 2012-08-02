DJANGO ON HEROKU

This repo was built by following the guide shown here:

https://devcenter.heroku.com/articles/django

There are some small modifications made to this project, which are listed below:

1) Project is default named "project". You can change this, but I wouldn't recommend it.
2) No apps installed whatsoever.
3) Uses gunicorn and a simple procfile to get started. Extendable easily, see Mike Tigas' work here:

http://v3.mike.tig.as/blog/2012/02/13/deploying-django-on-heroku/

4) You need git, heroku command line tools, virtualenv, and python to immediately get setup with this. 

---- How to Install ---

In the command line:

    $ git clone git://github.com/svsaraf/django_heroku.git
    $ cd django_heroku
    $ virtulenv venv
    $ source venv/bin/activate
    $ pip install -r requirements.txt

Test how everything works with:

    $ foreman start

And visit http://0.0.0.0:5000/ to see your new website!

To push to heroku, do the following:

    $ heroku create
    $ git push heroku master
    $ heroku open

If you have any questions, send me a note. It's easier if you understand what's going on, so if you're curious, read more in the git, django, heroku, and gunicorn documentation.

Best,
sanjay
