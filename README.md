Nginx Virtual server management script
===========

Bash Script for automating nginx virtual hosts creation and deletion.

## Installation ##

1. Download script

        $ git clone https://github.com/nbtdm/virtualhost.git

2. Enable it to be executed globally

        $ sudo mv virtualhost/nginxvhost /usr/local/bin/nginxvhost \
        && sudo chmod 755 /usr/local/bin/nginxvhost


## Usage ##

Basic command line syntax:

    $ sudo sh /path/to/nginxvhost [create | delete] [domain] [optional git repo]
    
With script installed on /usr/local/bin

    $ sudo nginxvhost [create | delete] [domain] [optional git repo]
    
This script will create a default user with the domain name without the tld as the username and password.
The public directory resides in /srv/http/ (e.g. /srv/http/google.com) and symlinked by public_html in home directory.
    

### Examples ###

to create a new virtual host:

    $ sudo nginxvhost create mysite.dev
  
to delete a virtual host

    $ sudo nginxvhost delete mysite.dev

