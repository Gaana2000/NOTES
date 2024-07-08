# DOCKER

**Docker** is a software platform that allows you to build, test, and deploy applications quickly. Docker packages software into standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime. Using Docker, you can quickly deploy and scale applications into any environment and know your code will run.


# Docker Hub

Docker Hub is a container registry built for developers and open source contributors to find, use, and share their container images. With Hub, developers can host public repos that can be used for free, or private repos for teams and enterprises.



### Dockerfile

A Dockerfile is a script that uses the Docker platform to generate containers automatically. It is essentially a text document that contains all the instructions that a user may use to create an image from the command line. The Docker platform is a **Linux-based platform** that allows developers to create and execute containers, self-contained programs, and systems that are independent of the underlying infrastructure. Docker, which is based on the **Linux kernel’s** resource isolation capabilities, allows developers and system administrators to transfer programs across multiple systems and machines by executing them within containers.

Docker containers may operate on any Linux host thanks to Dockerfiles. **Docker images** are used to construct container environments for applications, and they may be produced manually or automatically using Dockerfiles. Docker containers can execute Linux and Windows apps. Developers may use Dockerfiles to construct an automated container build that steps through a series of command-line instructions. Docker containerization is essentially virtualization at the operating system level. Without the startup overhead of **virtual machines**, several independent containers can run within a single Linux instance.

Dockerfiles provide business applications with more flexibility and mobility. Dockerfiles are used by IT companies to bundle programs and their dependencies in a virtual container that may operate on bare metal, in **public or private clouds, or on-premises**. Numerous apps, worker tasks, and other activities can operate independently on a single physical computer or across multiple virtual machines using containers. **Kubernetes** is an open-source solution for automating the management and orchestration of Dockerfile-based containerized applications.

**Commands in Dockerfile**

1. FROM
2. MAINTAINER 
3.  RUN
4. ADD
5. ENV
6. ENTRYPOINT
7. CMD

### Docker - Working with Containers

### docker top

With this command, you can see the top processes within a container.
 
**Syntax** - docker top ContainerID

● ContainerID − This is the Container ID for which you want to see the top processes.

**Return Value**
The output will show the top-level processes within a container.

●Example
**sudo docker top 9f215ed0b0d3**
 
The above command will show the top-level processes within a container.

### docker stop

This command is used to stop a running container.

**Syntax** - docker stop ContainerID 


● ContainerID − This is the Container ID which needs to be stopped.

**Return Value**
The output will give the ID of the stopped container.

● Example- sudo docker stop 9f215ed0b0d3 

The above command will stop the Docker container 9f215ed0b0d3.

### docker rm

This command is used to delete a container.

**Syntax**- docker rm ContainerID 

● ContainerID − This is the Container ID which needs to be removed.

**Return Value**
The output will give the ID of the removed container.

**Example**
sudo docker rm 9f215ed0b0d3 

The above command will remove the Docker container 9f215ed0b0d3.


### Docker Compose

Docker Compose is used to run multiple containers as a single service. For example, suppose you had an application which required NGNIX and MySQL, you could create one file which would start both the containers as a service without the need to start each one separately.

### Docker Compose ─ Installation

The following steps need to be followed to get Docker Compose up and running.

**Step 1** − Download the necessary files from github using the following command - 

**curl -L "https://github.com/docker/compose/releases/download/1.10.0-rc2/dockercompose
   -$(uname -s) -$(uname -m)" -o /home/demo/docker-compose**
   
The above command will download the latest version of Docker Compose which at the time of writing this article is 1.10.0-rc2. It will then store it in the directory /home/demo/.

**Step 2** − Next, we need to provide execute privileges to the downloaded Docker Compose file, using the following command −

**chmod +x /home/demo/docker-compose**

We can then use the following command to see the compose version.

**Syntax** -  **docker-compose version** 

**version** − This is used to specify that we want the details of the version of Docker Compose.

**Output**
The version details of Docker Compose will be displayed.

**Example**

The following example shows how to get the docker-compose version.

**sudo ./docker-compose -version** .


# How to write Dockerfile and Docker.yaml File

### STEP 1- SET UP

1. Create a directory for the project:

 **$mkdir composetest
    $cd composetest**

2. Create a file called app.py in your project directory 

3. Create another file called requirements.txt in your project directory:

flask
redis

4.Create a Dockerfile and paste the following code in:


 **syntax=docker/dockerfile:1**
FROM python:3.10-alpine
WORKDIR /code
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
RUN apk add --no-cache gcc musl-dev linux-headers
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
EXPOSE 5000
COPY . .
CMD ["flask", "run", "--debug"]

### STEP 2- DEFINE SERVICES IN A COMPOSE FILE

Compose simplifies the control of your entire application stack, making it easy to manage services, networks, and volumes in a single, comprehensible YAML configuration file.

Create a file called compose.yaml in your project directory and paste the following:


**services:
  web:
    build: .
    ports:
      - "8000:5000"
  redis:
    image: "redis:alpine"**
    
This Compose file defines two services: **web** and **redis**.

The **web** service uses an image that's built from the **Dockerfile** in the current directory. It then binds the container and the host machine to the exposed port, **8000**. This example service uses the default port for the Flask web server, **5000.**

The **redis** service uses a public Redis image pulled from the Docker Hub registry.

### STEP 3: BUILD AND RUN YOUR APP WITH COMPOSE

With a single command, you create and start all the services from your configuration file.

From your project directory, start up your application by running docker compose up.


 **$docker compose up**.
 
#  How to run Node.js apps inside Docker

▪Create a **Dockerfile**  file for an Express Node.js service container.

▪Build, run, and verify the functionality of the service.

▪Debug the service running within a container.


● Clone the sample application to use with this guide. Open a terminal, change directory to a directory that you want to work in, and run the following command to clone the repository:


 **git clone https://github.com/docker/docker-nodejs-sample**
 
 ● Inside the docker-nodejs-sample directory, run the docker init command in a terminal. docker init provides some default configuration, but you'll need to answer a few questions about your application. Refer to the following example to answer the prompts from docker init and use the same answers for your prompts.

**$docker init**
 
You should now have at least the following contents in your docker-nodejs-sample directory.


├── docker-nodejs-sample/
│ ├── spec/
│ ├── src/
│ ├── .dockerignore
│ ├── .gitignore
│ ├── compose.yaml
│ ├── Dockerfile
│ ├── package-lock.json
│ ├── package.json
│ └── README.md

To learn more about the files, see the following:
**Dockerfile**
**.dockerignore**
**compose.yaml**

● **Run the application in the background **

Inside the docker-nodejs-sample directory, run the following command in a terminal.

 **$docker compose up --build**
 
Open a browser and view the application at http://localhost:3000. You should see a simple todo application.

In the terminal, **press ctrl+c** to stop the application.

Run the application in the background,You can run the application **detached** from the terminal by adding the **-d** option. Inside the docker-nodejs-sample directory, run the following command in a terminal.

**$ docker compose up --build -d**
Open a browser and view the application at http://localhost:3000.

In the terminal, run the following command to stop the application.

  **$docker Compose down.