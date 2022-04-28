# Wordpress setup with Docker Compose and SSL - works on ARM

## Installation:

Before the installation, you need to update DNS records of your domain, i.e.:
```
Subdomain| Value| Record type | 
@	| <ip of the host> |	A 
www	| <ip of the host> |	A 
```

And then:

1. Clone the repository or copy these files to a machine you want to start WordPress
2. Setup Docker and Docker Compose (you can use the `install-docker.sh` installation script for Ubuntu).
3. Replace `EMAIL=youremail@something.com` and `URL=www.yoursite.com` in the docker-compose.yml file.
4. Run: `docker-compose up` or `docker-compose up -d` for the detached mode to run it in background.


Based on [docker-compose-wordpress-ssl](https://github.com/dawidkotarba/docker-compose-wordpress-ssl) and fantastic post:
[Quickly setup WordPress & SSL via Let’s Encrypt and Certbot using Docker Compose
](https://carlwillimott.medium.com/quickly-setup-wordpress-ssl-via-lets-encrypt-and-certbot-b29e8abf2072)