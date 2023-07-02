
# Docker 

## What is Docker 
Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. The service has both free and premium tiers. The software that hosts the containers is called Docker Engine.

## What is a docker image 
A Docker image is a read-only template that contains a set of instructions for creating a container that can run on the Docker platform. It provides a convenient way to package up applications and preconfigured server environments, which you can use for your own private use or share publicly with other Docker users.


## What is a docker container
Docker containers are the live, running instances of Docker images. While Docker images are read-only files, containers are life, ephemeral, executable content.



how to check docker images 

```docker
  docker images 
```

how to list docker containers 

```docker 
  docker ps 
```

how to download or pull docker image from registry

```docker
  docker pull {name}:{tag} 
  docker pull nginx:1.23
```
You can view the image by typing the below command

```docker
  docker images
```
Note if you pull an image without a specific tag, this is going to pull in the lastest image 

How to create a container from the give image 

```docker
  docker run {name}:
  docker run niginx:1.23
```
To to the container you just created run the below command 
```docker
  docker ps 
```
Detached mode, shown by the option --detach or -d , means that a Docker container runs in the background of your terminal. It does not receive input or display output.

how to run docker container in detach mode 
```docker
  docker run -d niginx:1.23
```

Checking container logs 
```docker
  docker logs {container_id}
```
Using docker run command 
this first looks for the image locally if it doesn't find it looks for it on docker hub, this downloads the image and run it at the same time.

```docker
  docker run {image}
```

how to stop a docker container 

```docker
  docker stop {container_id}
```

Point binding 

```docker
  docker run -d -p :9000:80 niginx:1.23
```
defaulty bhe nginx server is running on port 80 but now we have bind it to port 9000 so it now going to run on port 9000

## Naming a docker conatiner 

```docker
docker run --name {container-name} -d -p 9000:80 nginx:1.23
```

#### Building your own docker image using a DockerFile 

python is a docker file to run a python django application 
 
 ```docker
# Use an official Python runtime as a parent image
FROM python:3.9-slim-buster

# Set the working directory to /app
WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt .

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the current directory contents into the container at /app
COPY . /app

# Set environment variables
ENV PYTHONUNBUFFERED 1
ENV DEBUG 0

# Expose port 8000 for the Django app
EXPOSE 8000

# Run the command to start the Django app
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

```

Run the following command to build the image you have just created 

```docker
docker build -t {image_name} {location}
docker build -t django-app .
```

How to run the image in a container 

```docker
docker run -d -p 8000 django-app
```
