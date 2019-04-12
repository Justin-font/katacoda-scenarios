## Docker comp what ?
Docker compose is a tool for defining and running multi-container Docker applications.
You can define network to specify the connection between container, Env varriable, Volume.. all your application need.
- Volume ??? 
Sorry, volume allow you to  persist data into the container, it's like a link betwen the target file/folder in the contaier and the one one you're computer, for example you can modify your code on your conputer and with a voume.

## Lets compose
First analyse the docker-compose.yml file:
- `cat docker-compose.yml`{{execute}}
- `build` specify the path to the Dockerfile here . 
-  `ports` specify port for HOST:CONTAINER
-  `volume` specify linked forlder/file HOST:CONTAINER

Now we can start our docker-compose run : `docker-compose up -d --build`{{execute}}
- `docker-compose` we use docker-compose tool
- `up` to start all of the containers 
- `--build` to build the containers
You can add `-d` afeter `up` to run it in detached mode

Click on the cross on the top off the terminal and oppen **HTTP port 80**
It's the same result but with docker compose !
See the logs : `docker-compose logs`{{execute}}
Stop the compose : `docker-compose down`{{execute}}


Click on the cross on the top off the terminal and oppen **HTTP port 80**
Woaw the docker volume work !
