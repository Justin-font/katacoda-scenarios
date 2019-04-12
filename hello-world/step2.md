## So tell me more about your picture dock
Images, all is about images, in this comand : **docker run -ti ubuntu**
- docker run : is use to create a container
- -ti : to say hey i want to enter in the container shell
- ubuntu : the image that we use, here ubuntu, this image was ceated by docker but you can create an image of what you whant

## How can i create my own image
To create an image you need to write a **Dockerfile** whitch will tell to docker the steps to configure our image
Here we are going to create a web server withb nginx (nginx is avaible on any platform, it's the most used web server and have is official docker image `nginx`)
- Lets pull from git some examples  : `git clone https://github.com/Justin-font/Docker.git;  cd Docker/docker_examples/nginx `{{execute}}
- Lets analyse it : `cat Dockerfile`
- **From nginx** We specify the basic image here nginx
- **ADD index.html /usr/share/nginx/html** we add our html page in the root of the nginx server
This is the basic, in our Dockerfile we specify all that wee need to run our aplication, here you will install your dependencies for example and add your code.

## Now lets build and then run our image 
- Lets build the image : ` docker build --tag ngx .`{{execute}}
- - docker build to build the image 
- - --tag name the image here **ngx** 
- - . specify where your Dockerfile is locaed
- Lets run our image in a container : ` docker run --rm  -d -p 80:80 ngx `{{execute}}
- - docker run to run our container 
- - --rm to automatically remove the container when it exits
- - -d run container in background and print container ID
- - -p 80:80 Publish a container’s port(s) to the host
- - ngx the name of our image
- Click on the top of the terminal and select **View HTTP port 80**
- Woaw it just setup a server in 1 minutes, so fast 
## Stop the container
To continue this intro stop the container
- `docker container ls`{{execute}}
- the type : docker kill {{the container id of the inage ngx}}
## Have you meet docker-compose ?





Here you can find more information on Dockerfile https://docs.docker.com/engine/reference/builder/



