# Create a debian or ubuntu VM

# update the packages
```
su
apt update
apt upgrade
```

# install docker
```
apt install docker
apt install docker-compose
```

# Netbox docker image
```
git clone -b release https://github.com/netbox-community/netbox-docker.git
```

# copy the docker compose example
```
cp docker-compose.override.yml.example docker-compose.override.yml
cat docker-compose.override.yml
```

# pull the images
```
docker-compose pull
```

# run the images
```
docker-compose up -d
```

# create superuser account
```
docker-compose exec netbox /opt/netbox/netbox/manage.py createsuperuser
```
