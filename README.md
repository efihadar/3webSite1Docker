# 3webSite1Docker

About this image
This image is a NGINX reverse proxy which generates a self-signed certificate and is configured for TLS1.3 by default.

Possible ENV variables
FRWRD_TO - address of the machine you want to forward to.

EXT_ACCESS - setting any value will add to the generated certificate the public IP address of the server.

To run it with docker run
docker run -e FRWRD_TO=10.0.0.1:4444 -d  -p 80:80 -p 443:443 macie/sslproxy
