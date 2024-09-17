# Create directory
mkdir compose
cd compose/

# docker compose command
````
docker compose
````
# Download docker-compos.yml file for vprofile project
````
wget https://raw.githubusercontent.com/devopshydclub/vprofile-project/docker/compose/docker-compose.yml
ls
vim docker-compose.yml
````

# Bring up all the containers
````
docker compose up -d
docker compose ps
ip addr show | grep inet
docker compose down
docker stop $(docker ps -a --format '{{.Names}}')
docker rm  $(docker ps -a --format '{{.ID}}' )
docker rmi $(docker images --format '{{.ID}}')
````

Go to browser and enter VMIP:80
