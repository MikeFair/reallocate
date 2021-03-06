ReAllocate Web Platform 
============================
This open source project is for the ReAllocate (reallocate.org) marketplace, where knowledge meets need.

PREREQUISITES

- Python 2.7
- pip (Python)
- SQLite
- XCode or CLI (Mac OS X)

INITIAL SETUP

- git clone git@github.com:reallocate/reallocate.git
- (OPTIONAL: use [virtualenv](http://www.virtualenv.org/) to create an isolated python environment for your ReAllocate development)
- sudo pip-2.7 install -r requirements.txt (if using a virtualenv, omit sudo)
- create a settings_local.py file next to settings.py
- ./manage.py syncdb --all  (It will ask to create a superuser; answer "yes" -- and use admin / admin for consistency)
- ./manage.py runserver

OPTIONAL SETUP

If you want to be able to connnect to AWS, Google, LinkedIn, etc you will need to add those keys. To do so:

- create website/settings_local.py
- put all your overrides in there.  if you are a ReAllocate core team member, you can find this file in our Dropbox
