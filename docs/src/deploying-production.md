# Preparing the server

```
ssh usernamr@server_ip

sudo apt install docker-compose docker.io git make

```

# Getting the code source

```
cd ../
sudo mkdir bims
sudo chown kartoza:kartoaz bims
cd bims
git clone https://github.com/kartoza/django-bims.git

```

# Build docker images

```
cd deployement
cp docker-compose.override.template.yml docker-compose.override.yml
cd ../
make web

```