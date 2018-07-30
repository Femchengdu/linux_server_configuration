# linux_server_configuration
Configuring an Ubuntu 14.04 Linux Server on Digital Ocean

### Project Specifications:

IP : 178.128.70.181
SSH Port : 2200
Complete URL: http://178.128.70.181.xip.io
 
## Summary of software and configuration changes.

#### Steps Taken:
* apt-get update
* apt-get upgrade
* adduser catalog and grader
* installed finger
* added grader and catalog to the sudoers list
* created ssh files for the grader(pass_phrase: final_project) and student
* restarted ssh service
* logged out as root
* logged in as catalog
* ufw configured with ssh, http, and ntp
* installed apache2
* installed mod-wsgi
* Installed git
* Installed python-dev
* update upgrade and auto remove
* clone the GitHub files
* copied the catalog from repository to /var/www/catalog
* renamed application.py to __init__.py
* removed host and port from app.run()
* installed python-pip
* installed the virtual env
* installed the virtual env in /var/www/catalog/catalog/catalog_env/
* activated the catalog_env
* installed flask
* added catalog.conf with http://178.128.70.181.xip.io 
* ran sudo a2ensite catalog
* ran sudo service apache2 reload to activate
* created catalog.wsgi and added secret key: chengdu_ruby_python
* ran sudo service apache2 restart
* Installed postgresql
* database created with owner catalog
* granted all privileges on the database to catalog
* created the catalog db to enable login without passowrd(don't know if I need this)
* activated the virtual environment
* ran pip install SQLAlchemy
* deactivate the virtual environment
* ran sudo apt-get install python-psycopg2
* activated the virtual environment
* ran sudo pip install --upgrade google-api-python-client
* ran sudo pip install google-auth-oauthlib
* modified the database for postgresql with username and password
* modified database_setup.py and tested
* modified lotsofskill.py and populated the database
* enabled ssl
* deactivated the root user login

