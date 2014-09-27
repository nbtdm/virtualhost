Nginx Virtual server management script
===========

Bash Script for automating nginx virtual hosts creation and deletion.

## Installation ##

        $ git clone https://github.com/nbtdm/virtualhost.git /tmp/virtualhost \
        && sudo cp /tmp/virtualhost/nginxvrhst /usr/local/bin/nginxvrhstnginxvrhst \
        && sudo chmod 755 /usr/local/bin/nginxvrhst && rm -Rf /tmp/virtualhost



## Usage ##

Basic command line syntax:

    $ sudo sh /path/to/virtualhost.sh [create | delete] [domain] [optional host_dir]
    
With script installed on /usr/local/bin

    $ sudo virtualhost [create | delete] [domain] [optional host_dir]
    

### Examples ###

to create a new virtual host:

    $ sudo virtualhost create mysite.dev
  
to create a new virtual host with custom directory name:

    $ sudo virtualhost create anothersite.dev my_dir
  
to delete a virtual host

    $ sudo virtualhost delete mysite.dev
  
to delete a virtual host with custom directory name:

    $ sudo virtualhost delete anothersite.dev my_dir
