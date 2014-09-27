Nginx Virtual server management script
===========

Bash Script for automating nginx virtual hosts creation and deletion.

## Installation ##

        $ git clone https://github.com/nbtdm/virtualhost.git /tmp/virtualhost \
        && sudo cp /tmp/virtualhost/nginxvrhst /usr/local/bin/nginxvrhstnginxvrhst \
        && sudo chmod 755 /usr/local/bin/nginxvrhst && rm -Rf /tmp/virtualhost



## Usage ##

Basic command line syntax:

    $ sudo sh /path/to/virtualhost.sh [create | delete] [domain] [optional git repo]
    
With script installed on /usr/local/bin

    $ sudo virtualhost [create | delete] [domain] [optional git repo]
    
This script will create a default user with the domain name without the tld as the username and password.
The public directory resides in /srv/http/ (e.g. /srv/http/google.com) and symlinked by public_html in home directory.
    

### Examples ###

to create a new virtual host:

    $ sudo virtualhost create mysite.dev
  
to delete a virtual host

    $ sudo virtualhost delete mysite.dev

