- docker run will start a new container
- docker start will start an existing container

docker run --name myapp_c_nodemon -p 4000:4000 --rm -v "C:\Users\tanan\Desktop\Github Repos\simple-docker-app\api:/app" -v "/app/node_modules" myapp:nodemon
    - This will start a new container named myapp_c_nodemon, mapping port 4000 to 4000
    - Remove the container when it stops from the image myapp:nodemon
    - Mount the volume C:\Users\tanan\Desktop\Github Repos\simple-docker-app\api to /app
    - Mount the volume /app/node_modules, prevents node_modules in container from being overwritten by the host's node_modules

////////////////////////////////////////////////////////////////////////////////////////////////
docker-compose up
    - This will start the containers defined in docker-compose.yaml
    - using docker-compose down --rmi all -v
        - will stop the containers and remove volumes and image created by docker-compose up

