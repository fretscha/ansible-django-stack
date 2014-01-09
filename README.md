ansible-django-stack
====================

Goal of this project is to deploy the entire django stack with help of ansible

todo
----
* My First 5 Minutes On A Server
* Database setup
  * Christophe Pettus's PostgreSQL configuration
    * Logging
    * Memory
    * Checkpoint
    * Planner
* Python Layer
  * pip
  * virtualenv
  * django
* Application
  * git pull django project
  * install requirements
* uWSGI Appserver
* Gunicorn Appserver
* Supervisord
* Apache reverse proxy
  * apache 2.4
  * mod_security
* Nginx reverse proxy
* Caching
  * memcached
* Loadbalancer
  * HAProxy

My First 5 Minutes On A Server
------------------------------
1. Update & upgrade the system via apt-get
2. Reset our root password to something strong
3. Create a new user so we don't have to use root
4. Copy over our pub key
5. Lock down sudo
6. Lock down ssh to prevent root & password login
7. Setup the ufw firewall
8. Install vim, ntp, postfix
9. Install fail2ban to block attacks
10. Configure unattended security upgrades
11. Configure logwatch to email daily server logs
