# p5-linux-server-configuration
FWDN p5

IP 52.36.92.37  
URL ec2-52-36-92-37.us-west-2.compute.amazonaws.com  
SSH port 2200  

## Installed software
pip, virtualenv, Apache + mod_wsgi, PostgreSQL, Git + numerous Python modules and libraries (python-psycopg2, flask, python-sqlalchemy, oauth2client, requests, httplib2...)

## Configuration
After setting up user privilleges, SSH and ports configuration and intalling additional software (Apache, PostgreSQL, Git) Catalog App had been cloned into /var/www/ directory.  
mod_wsgi installation process required some changes in directory structure, replacing SQLite3 database with PostreSQL one, and adding config file in /etc/apache2/sites-available/ to make our app accessible.  
Also, Google Sign In script needed some changes - server IP and URL have been added to origin section.
