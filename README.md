# docker-nginx-letsencrypt
Docker image with Nginx setup using Lets encrypt SSL encryption and a few apps (jenkins, ...)

- Create subdomain for Jenkins pointing to a valid public IP address
- Open port 80 and 443 on server
- Create htpasswd file in order to use basic authentication for your endpoints. Place the created file in a folder named htpasswd: 
Example og basic authentication for the domain name example.com and for user: htpasswd -c example.com user

htpasswd needs apache2-utils to be installed on your machine
Documentation for htpasswd: http://httpd.apache.org/docs/2.2/programs/htpasswd.html

Note: the folder htpasswd is mounted in the docker container.
