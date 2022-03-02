Install Certbot Cloudflare DNS
=========

The role installs certbot on an Ubuntu host and sets up Cloudflare DNS Challenge.

Usefull if one, wants to use real Let's Encrypt certificates in a homelab.

Requirements
------------

None

Role Variables
--------------

### Credentials
Credentials have to be provided in an .ini file. See https://certbot-dns-cloudflare.readthedocs.io/en/stable/#credentials for reference. <br>

### Domain
The domain you want to have a certificate for. <br>
Example: **myvpn.atmyhome.com**

### Email
Email for address for ACME update

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - install-certbot-cloudflaredns
      vars:
        credentials: ~/cloudflare.ini
        domain: myvpn.atmyhome.com
        email: coolguy@example.com

License
-------

MIT