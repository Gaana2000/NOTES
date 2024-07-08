# AWS

**Amazon Web Services (AWS)** is a leading top platform in providing the web services of various domains. AWS follows the trends of digital IT and comes up needy services with optimized performances covering a wide range of services from Compute to Storage. It covers a wider range of customers of different domains to expand their business operations. This Article covers the fundamentals of AWS and its scope of IT business.

● AWS stands for Amazon Web Services, It is an expanded cloud computing platform provided by Amazon Company. AWS provides a wide range of services with a pay-as-per-use pricing model over the Internet such as Storage, Computing power, Databases, Machine Learning services, and much more. AWS facilitates for both businesses and individual users with effectively hosting the applications, storing the data securely, and making use of a wide variety of tools and services improving management flexibility for IT resources.

**How AWS Works?**

AWS comes up with its own network infrastructure on establishing the datacenters in different regions mostly all over the world. Its global Infrastructure acts as a backbone for operations and services provided by AWS. It facilitates the users on creating secure environments using **Amazon VPCs ( Virtual Private Clouds )**. Essential services like **Amazon EC2** and **Amazon S3** for utilizing the compute and storage service with elastic scaling. It supports the dynamic scaling of the applications with the services such as Auto Scaling and **Elastic Load Balancing ( AWS ELB )**. It provides a good user-friendly AWS Management Console facilitating seamless configuration and management of AWS services to the Users. Its Architecture ensures high availability , fault tolerance making AWS as a versatile powerful Cloud Computing Platform.


# AWS Fundamentals

In the Journey of AWS, understanding the key concepts such as Regions, Availability Zones, Global Network Infrastructure, etc is crucial. The fundamentals of AWS keep on maintaining the applications reliable and scalable with services globally with coming to a strategic deployment of resources for optimal performance and resilience. The following are the some of the main fundamentals of AWS:

1. **Regions**: 
AWS provide the services with respective division of regions. The regions are divided based on geographical areas/locations and will establish data centers. Based on need and traffic of users, the scale of data centers is depended to facilitate users with low-latencies of servcies.

2. **Availability Zones (AZ)**: 
To prevent the Data centers for the Natural Calamities or any other disasters. The Datacenters are established as sub sections with isolated locations to enhance fault tolerance and disaster recovery management.

3. **Global Network Infrastructure**: 
AWS ensures the reliability and scalability of services through setting up its own
**AWS Network Infrastructure**
globally. It helps in better management of data transmissions for optimized performance and security reliance.


# Top AWS Services

In the rapid revolution of Cloud Computing, AWS facilitates with wide variety of services respect to the fields and needs. 

1. **Amazon EC2(Elastic Compute Cloud)**

 It provides the Scalable computing power via cloud allowing the users to run applications and manage the workloads over their remotely.
 
2. **Amazon S3 (Simple Storage Service )**:

It offers scalable object Storage as a Service with high durability for storing and retrieving any amount of data.

3. **AWS Lambda**:

It is a service in Serverless Architecture with Function as a Service facilitating serverless computing i.e., running the code on response to the events, the background environment management of servers is handled by aws automatically. It helps the developers to completely focus on the logic of code build.

4. **Amazon RDS (Relational Database Service)**:

This is an aws service that simplifies the management of database providing high available relational databases in the cloud.

5. **Amazon VPC (Virtual Private Cloud)**:

It enables the users to create isolated networks with option of public and private expose within the AWS cloud, providing safe and adaptable configurations of their resources.


# Advantages Of Amazon Web Services

● AWS allows you to easily scale your resources up or down as your needs change, helping you to save money and ensure that your application always has the resources it needs.
 
● AWS provides a highly reliable and secure infrastructure, with multiple data centers and a commitment to 99.99% availability for many of its services.

● AWS offers a wide range of services and tools that can be easily combined to build and deploy a variety of applications, making it highly flexible.

● AWS offers a pay-as-you-go pricing model, allowing you to only pay for the resources you actually use and avoid upfront costs and long-term commitments.
 
# Disadvantages Of Amazon Web Services

● AWS can be complex, with a wide range of services and features that may be difficult to understand and use, especially for new users.

● AWS can be expensive, especially if you have a high-traffic application or need to run multiple services. Additionally, the cost of services can increase over time, so you need to regularly monitor your spending.

● While AWS provides many security features and tools, securing your resources on AWS can still be challenging, and you may need to implement additional security measures to meet your specific requirements.

● AWS manages many aspects of the infrastructure, which can limit your control over certain parts of your application and environment.


# Applications Of AWS

The AWS services are using by both startup and MNC companies as per their usecase. The startup companies are using overcome hardware infrasture cost and applications deployments effectively with cost and performance. Whereas large scale companies are using AWS cloud services for the management of their Infrastructure to completely focus on the development of products widely. The following the Real-world industrial use-cases of AWS services:

**Netflix** :

 The Large streaming gaint using AWS for the storage and scaing of the applications for ensuring seamless content delivery with low latency without interruptions to millions of users globally.
 
**Airbnb** : 

By utilizing AWS, Airbnb manages the various workloads and provides insurable and expandable infrastructure for its virtual marketplace and lodging offerings.

**NASA’s Jet Propulsion Laboratory** : 

It takes the help of AWS services to handle and analyze large-scale volumes of data related to vital scientific research missions and space exploration.

**Capital One** : 

A financial Company that is utilizing AWS for its security and compliance while delivering innovative banking services to its customers.

# PUSH DOCKER IMAGE

By pushing an image to the DockerHub registry, we can create an instance of an image in which a particular type of software and applications are pre-installed and can be pulled again whenever you want to work on that particular type of image or application and run that kind of virtual machine. In the DockerHub there are millions of images you can also pull the default images which are created by particular organizations for example you can pull the Ubuntu image which is uploaded by Linux, and then install any software or application into that image like curl command, Jenkins, etc and then push that docker image to your docker hub registry. 

**Docker push is a command which is used to push the docker images to the docker Private/Public registries**. After building the customized docker image you need to push it to the remote registries from where other developers or DevOps engineers can access the image and work on it to push the image you can use the docker push command. It is an important step to perform because if you store it locally others can’t access the image but if it is available remotely others can access it.

**Docker Push Command**

Docker push commands requires two arguments to push the command into the registry.They are

▪ Name of the Docker image.

▪ Name of the registry to push the image.

**Example**:

If you want to push an image with the name as **GFG-Image** to the **GFG-DockerImages** repository which is located in the dockerhub registry then you will use the following command.

**docker push GFG-Image GFG-DockerImages** 

**docker push  <Name of the image> <Name of the repo>**

In the place of **<Name of the image>** replace with your image name and in the place of **<Name of the repo>** replace with the your repository name.


# PULL DOCKER IMAGE

You can pull any type of docker image by using the command docker pull. Along with the command you need to mention the image name that you want to pull for example

If i want to pull the docker image nginx then you use the command.

**docker pull nginx** 

You can use different other flags with the command like — flag name of the flag.

**How to run a Docker Container**

To use the **docker run** command, you must specify the image’s name to be executed. Additionally, the command that will be run within the container can be given.

To execute the echo **“Hello, world!”** command inside the container, the following command gives you to run the most recent version of the Ubuntu image:

**docker run ubuntu echo "Hello, world!"**

The docker run command initiates a new container and executes the specified command within it. The container will continue running until the command completes.


# How Does the Pull Command Work in Docker?

When the Docker pull command is executed, several steps are involved in the process of acquiring the requested container image. Some of them are defined further:

1. **Identification of the Image** –

  The first step is to identify the specific image to be pulled. This is done by specifying the image name along with its repository and optionally a tag that represents a specific version or variant of the image. For example, to pull the official NGINX image from Docker Hub, the command would be **`docker pull nginx`**.

2.  **Contacting the Docker Registry** –

Once the image name is identified, the Docker daemon contacts the Docker registry specified in the image name (e.g., Docker Hub). The registry is a centralized repository that stores and distributes Docker images. By default, Docker Hub is the public registry, but private registries can also be utilized.

3. **Authenticating and Authorizing** – 

If the registry requires authentication and the user has not previously logged in, the Docker daemon prompts the user to provide valid credentials. The authentication process ensures that only authorized users can access private or restricted images.

4. **Requesting the Image Manifest** –

 After the authentication process, the Docker daemon sends a request to the registry for the image manifest. The manifest contains metadata about the image, such as the layers that compose it, its dependencies, and other configuration details. The manifest allows Docker to understand how to assemble and run the container based on the pulled image.

5.  **Downloading Image Layers** – 

Once the manifest is received, the Docker daemon starts downloading the image layers one by one. Docker uses a layered architecture, where each layer represents a specific part of the image’s filesystem. Layers are stacked on top of each other, allowing for efficient storage and sharing of common layers across multiple images. Docker downloads and verifies each layer’s integrity before moving on to the next.

6. **Assembling the Image**  – 

 As the layers are downloaded, Docker progressively assembles them into a complete image based on the instructions provided in the manifest. Each layer contributes to the final filesystem state and configuration of the container. The layering approach allows for quick and efficient updates since only the modified or new layers need to be downloaded and applied.

7. **Image Caching** – 

To optimize the pulling process, Docker caches downloaded layers locally on the host machine. When subsequent pulls of the same image or images with shared layers are performed, Docker can utilize the cached layers, significantly reducing download times. The cache is periodically updated and can be managed using Docker’s caching mechanisms.


# Difference between Docker Image and Docker Container


**Docker Image and 	Docker Container**

1. It is a blueprint of the Container.	It is an instance of the Image.

2. Image is a logical entity.	The container is a real-world entity.

3. Images are created only once.	Containers are created any number of times using an image.

4. Images are immutable. One cannot attach volumes and networks.	Containers change only if the old image is deleted and a new one is used to build the container. One can attach volumes, networks, etc.

5. Images do not require computing resources to work.	Containers require computing resources to run as they run with a Docker Virtual Machine.

6. To make a docker image, you have to write a script in a Dockerfile.	To make a container from an image, you have to run the **“docker run <image>”** command.

7. Docker Images are used to package up applications and pre-configured server environments.	Containers use server information and a file system provided by an image in order to operate.

8. Images can be shared on Docker Hub.	It makes no sense in sharing a running entity, always docker images are shared.

9. An image must not refer to any state to remove the image.	A container must be in a running state to remove it.

10. One cannot connect to the images as these images are like snapshots.	In this, one cannot connect them and execute the commands.

11. Sharing of Docker Images is possible.	Sharing of containers is not possible directly.

12. It has multiple read-only layers.	It has a single writable layer.

13. These image templates can exist in isolation.	These containers cannot exist without images.

14. There is no such thing as a running state of a Docker Image.	Containers use RAM when created and in a running state.