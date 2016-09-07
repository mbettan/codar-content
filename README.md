# HPE CODAR Contents - OpenLDAP

This project provides additional Docker Containers for HPE Codar :
- OpenLDAP - LDAP Server with sample data for CODAR RBAC
- phpldapadmin - LDAP Client to browse sample data and modify

# Docker Compose 
wget https://raw.githubusercontent.com/mbettan/codar-content/master/docker-compose.yml
docker-compose up

# Docker Engine
docker run -d -p 389:389 -e SLAPD_PASSWORD=admin -e SLAPD_DOMAIN=example.com mbettan/codar-openldap:latest

