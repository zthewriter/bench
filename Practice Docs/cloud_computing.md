# Cloud Computing Notes 
## Technical Writing Bootcamp

## Overview of Cloud Computing 

- Basic Architecture of a Computer 
- What is Cloud Computing? 
- Advantages of Cloud Computing 

## Basic Architecture of a Computer 

- CPU - Central Processing Unit
  - This is the brains of the computer. All the processing is done here. All logical operations are done here. 
- Memory (RAM) 
  - Random Access Memory 
  - Data storage while the computer is running 
  - Non-persist storage because all the data stored in here is lost once the computer shuts done 
  - It is high speed storage that you can access while the computer is running  
- HDD
  - Hard Disk Drive 
  - Persistent storage device 
  - When you turn on your computer, the data will still be there
  - The Operating System is stored here
- NIC
  - Network Interface Card
  - This allows you to connect to internet and the external world 

## What is Cloud Computing? 

The official definition is: 

>Cloud computing is the **on-demand availability** of computer resources and IT services from a third-party provider through a network such as the Internet. 

This means that you don't actually own the infrastructure that these services are running on. In a sense, everything is already taken care of for you by a third party Cloud Computing provider. You hire or rent this third party. This changes provider to provider. Either way you will pay a subscription fee or a pay-what-you-use service. You can access these services when you want them. You pay for the time and capactiy that you use. 

On-premise data center (opposite of cloud computing)
- You will need to shrink these servers manually when you experience lower demand 
- This is not made to scale 
- Cloud computing is made to SCALE 

## Advantages of Cloud Computing 

- Trade fixed expense for variable expense 
  - Pay only for what you consume
  - Variable expense, the more you use, the more you pay. The less you use, the less you pay. 
  - Benefit from massive economies of scale 
    - The more clients a company has, and the more effecient it is with operations, the lower it can lower prices 
  - Stop guessing capacity 
    - Scale within minutes to meet capacity needs 
  - Increase speed and agility 
    - IT resources are a click away 
    - Instead of having tools available to developers in weeks, have tools available in minutes 
    - Dramatic increase in agility 
  - Stop spending money running and maintaining data centers 
    - Stop paying for server maintenance 
  - Go global in minutes 
    - Data centers all over the world 
    - Provide lower response times (latincy?)

## Infrastructure in the Clould 

- Virtual Servers 
- Containers 
- Storage Services 
- Databases 
- Networking (the ghost element in the infrastructure of the cloud)

## Virtual Servers 

Virtual servers include the following characteristics: 
- Separated instances (entities that compute) from the physical server 
- One operating system for each virtual machine 
  - These are separate from the physical server 
  - You can have many virtual machines running on the same server 
  - The virtual machine lives on top of the server as its own element 
  - The **hypervisor** software virtualizes the hardware 
  - Each virtual machine has its own operating system 
    - Each virtual machine also has its own RAM, NIC, CPU, and HDD
## Containers 
- **Containers** include the following characteristics: 
  - Packaged software into isolated units 
  - Shared operating system from the physical server 
  - One operating system for all the different containers 
  - Containers hold different software. For example, one container will hold Python while another container holds JavaScript. The key note here is that they all exist together in the same Operating System. 
  - Also, this is all possible thanks to the Docker Engine which lives inside the operating system 
  - **Docker Engine**: It is a technology to build and containerize your applications
  - Containers are very fast and agile  

> Key difference between Virtual Machines and Containers: 
> Virtual Machines virtualize the hardware components of a computer to run virtually (for example elements such as CPU, NIC, etc.) Containers provide a way to virtualize an operating systems so multiple workloads and software can run on the same operating system. 

## Storage Service 

- **File storage:** A piece of data is saved inside of a folder  
- **Block storage:** Chops data into blocks and saves them in different sources. Keep data apart and reattach it later.  
- **Object storage:** Files are broken into pieces and you are presented with only 1s and 0s. This is good for unstructured data. Discreet objects are called objects.  

## Databases 

A **database** is an **organized collection** of structured information or data. 

The most common databases are called **relational databases**. This is rows and columns in tables. You can retrieve the files easily. 

**Non-relational databases** do not use tables. They use storage model made for your data. For example, JSON is a format. 

**Graph databases**, such as used in Facebook, exist also. 

## Cloud Computing Models 

### Service Models 
  - Infrastructure as a Service (IaaS)
  - Platform as as a Service (PaaS)
  - Software as a Service (SaaS)
### Deployment Models
  - Public Cloud 
  - Private Cloud 
  - Hybrid Cloud  

> Deployment means building and developing an application and making it available to users. Bascially, buillding a software and pushing it to production. 

Infrastructure as a service (severs only) 
- Offers a way to get computing capabilites 
- Storage facilities 
- Network 
- Processing power 
- Physical capabilites 
- You don't need to manage the Infrastructure, this means the cloud provider is giving you the hosting infrastructure 
- Key word: host 
- You are responsible to manage and configure the operating systems 

Platform as a Service (servers and operating system) 
- Access to cloud based envrionments 
- The Cloud Provider offers the Servers and Operating Systems 
- This is a great solution for developers 
- Key word: build 
- You only care about building the application 

Software as a Service (servers, operating system, and applications) 
- The Cloud Provider owns everything 
- Relieves your organization from the constant pressure of maintaining operatational issues with keeping your applications up and runnung 
- You are only consuming the application content
- Key word: consume 

## Cloud Computing Deployment Models 

You have three options to deploy everything to the Internet:
- Public Cloud: You do not own any hardware. All resources are provided to you by a Cloud provider. This is the most common "Cloud". Examples: AWS, Googgle Cloud, Microsoft Azure 
- Hybrid Cloud: Somewhere inbetween the public and private cloud. 
- Private Cloud: On-premise data centers. Hardware is yours, you own everything. 

## Cloud Providers (Big Players)

- Amazon Web Services (AWS)
- Microsoft Azure (Azure)
- Google Cloud Platform (GCP) 

AWS is for medium and large enterprises requiring a versatile solution with customization and expansion freedom. The biggest cloud provider in the world with 33% market share. 

Azure the second largest cloud provider in the world with a market share of 13%. Azure is for small and medium companies requiring a system reinforced by a Microsoft ecosystem. 

GCP is for small companies or separate goals and needs that require cost-effective smart tools and cloud optimization features. GCP has 5% market share. 

This presentation will focus on AWS. Maybe companies are migrating to AWS cloud provider. 

## AWS Basics 

What makes AWS a leading cloud platform? 

- AWS Global Infrastructure 
  - AWS has many data centers all over the world 
  - AWS has many regions world wide 
  - Your data can become replicated and sent to another data center in the event of natural disaster for example an earthquake 
  - Make faster connections by selecting a data center near you 

- AWS offers over 18,000 services 
  - Computing 
  - Storage solutions 
  - Cloud app and integration 
  - Analytics and machine learning 
  - Productivity tools 
  - Developer and management tools 

## AWS Services Highlights 

Imagine this use case: 

A company wants to use their computer hardware, use IaaS (so server only with full control of applications and the operating system), and a Virtual Machine. 

AWS has a solution that meets all these conditions. It is called Amazon EC2 (Elastic Compute Cloud). 

You pay per second 

Imagine you want to store media files. You want people to be able to search for the images in the web. But, you want them to be secure. 

AWS has a solution for this too. Amazon S3 (Simple Storage Service)

Media files are objects. 

You can store your objects in buckets. 

## AWS Services Highlights 

### Databases 
- Amazon Aurora 
- Amazon Relational Database Service 
- Amazon DynamoDB
- Amazon Redshift 

### Containers 
- Amazon Elastic Container Service 
- Amazon Elastic Kubernetes Service 
- AWS Fargate 

### Storage 

- Amazon Elastic File System
- Amazon Elastic Block Store 
- AWS Storage Gateway 

### Machine Learning 

- Amazon Polly: Converts writter text to speech
- Amazon Rekognition: Recognizes images and videos that you input  
- Amazon SageMaker: Software that enables developers to optimize their machine learning models  











