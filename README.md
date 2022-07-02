# Ubuntu-Docker-constant
### Keep an Ubuntu container open indefinitely.

## How it works.
The script itself exists with in the dockerfile(Testing-Env)

It runs with a simple sleep command and it is supposted to go on forever, so that you can enter it.


# Instalation 
Download or copy the file contents into their apropreatly named files.

## Build the image
````
docker-compose -f Testing-Env.yml build
````

## Start the container
````
docker-compose -f Testing-Env.yml up -d
````

### Oneliner to build the image and start the container.
````
docker-compose -f Testing-Env.yml build && docker-compose -f Testing-Env.yml up -d
````

Enter the container to mess arround:
````
docker exec -it Testing-Env /bin/bash
````
