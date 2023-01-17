# Environment config
## Install docker

# Tutorial
### [Video](https://www.youtube.com/watch?v=PGL1D_Lv2FU)

## Docker references
[Cheat sheet](https://github.com/subhrendu1987/DockerCommandReferences/blob/main/README.md)

# Configuration
1. Change `docker-compose.yaml` with proper credentials
1. Change `ports:` of service named `phpldapadmin:` as per your conven

## Build and Execute
```
# Dependent dockers
#cd myLabLDAP/docker-openldap/docker-light-baseimage
#make
#cd ../
#make
mkdir -p data
sudo docker-compose pull
sudo docker-compose up -d
```
Use web browser to navigate to [http://127.0.0.1:8081/](http://127.0.0.1:8081/). Default admin username and password can be found in `docker-compose.yaml` (i.e. `LDAP_ADMIN_USERNAME=admin`,`LDAP_BASE_DN=dc=ucllocal,dc=com`,`LDAP_ADMIN_PASSWORD=admin_pass`) Use admin in the following format `cn=admin,dc=ucllocal,dc=com`
