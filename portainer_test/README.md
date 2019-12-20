
# Portainer 
docker volume create portainer_data
docker run -d -p 9000:9000 -p 8000:8000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer

# docker-compose
Please run ` docker-compose -d up` to start the serice and `docker-compose down` to stoped it
