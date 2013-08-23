## Flask Login OpenShift Quickstart##

A simple todo application built using Python 2.6 , Flask , Flask-SQLAlchemy , Flask-Login, PostgreSQL 9.2 , and Twitter Bootstrap.

1. Create the application using 
```
$ rhc app create todo python-2.6 postgresql-9.2
```

2. Pull the source code from github
```
$ cd todo
$ git rm -rf wsgi/ setup.py setup.pyc setup.pyo 
$ git commit -am "deleted default source code"
$ git remote add upstream -m master https://github.com/shekhargulati/flask-login-openshift-quickstart.git
$ git pull -s recursive -X theirs upstream master
```

3. Push the application to OpenShift
```
$ git push
```
