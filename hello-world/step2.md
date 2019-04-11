## So tell me more about your picture dock
Images, all is about images, in this comand : **docker run -ti ubuntu**
- docker run : is use to create a container
- -ti : to say hey i want to enter in the container shell
- ubuntu : the image that we use, here ubuntu, this image was ceated by docker but you can create an image of what you whant

## How can i create my own image
You can do it with a **Dockerfile**
- Lets pull from git some examples : `git pull ` {{execute}}
- Lets build the image : ` cd Docker/nginx; docker build --tag ngx .` {{execute}}
- Lets run our image in a container : ` docker run --rm  -d -p 80:80 ngx `{{execute}}
- Click on the top of the terminal and select **View HTTP port 80**
- Woaw it just setup a server in 1 minutes, so fast 

## What have we done ?
- We created our own image of nginx with our **Dockerfile** 
- Lets analyse it : `cat Dockerfile`
- **From nginx** We specify the basic image here nginx
- **ADD index.html /usr/share/nginx/html** we add our html page in the root of the nginx server
This is the basic, in our Dockerfile we specify all that wee need to run our aplication, here you will install your dependencies for example and add your code.

Here you can find more information on Dockerfile https://docs.docker.com/engine/reference/builder/



