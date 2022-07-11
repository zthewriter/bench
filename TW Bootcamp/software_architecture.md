# Software Architectures 
This document will discuss: 
- Understand the concept of software architecture 
- Identify a software architecture diagram 
- Learn how-to document a software architecture guide 

## What is **not** a software architecture? 

- An architecture **does not** include all the design decisions in a single view 
- An architecture **does not** inlude all the components, their functionality, and their interaction with other components in a single view. 
- An architecture **does not** describe in detail the building design 

## What is a software architecture? 

"A **software architecture** refers to the fundamental structures of a **software system** and the discipline of creating such structures and systems. Each structure comprises software **elements**, **relations** among them, and **properties** of both the elements and the relations" 

This quote comes from the book "Documenting Software Architectures: Views and Beyond" 

Software Architecture = 
- Elements 
- Relationships 
- Properties 


The Frontend, Backend, and Database are all inside the larger component called the Server. 

Amazon CloudFront is in the Frontend

The Database has an RDS DB instance. And Amazon ElasticCache. 

The Backend include Elastic Load Balanaceing. And a Bucket. And a Web Server and App Server. 

There are different view for different audiences. 

View 1 - Context 
View 2 - Containers 
View 3 - Components 

## How to Document a software architecture 

"Documenting an architecture is a matter of documenting the relevant views and then adding documentation that applies to more than one view" 

### Template for a technical audience 

Includes these components: 

- Overview 
- High-level diagram 
- Frontend 
  - Properties 
  - Relationships 
- Backend 
  - Properties 
  - Relationships 
- Database 
  - Properties 
  - Relationships 

A more detailed template:
Explain the container and then explain the relationships and properties of those containers. 

- Deinfe all the elements as a first step 

### Example Overview: 

YouTube is a web application that delivers videos to end-users. Users can upload their content and also view videos uploaded by other users. 

The YouTube application is a cloud-based platform that includes the following main components: 
- End User: Requests content through a user interface. 
- Frontend: Displays the content requested by the end-user 
- Backend: Handles frontend requests and retrieves content from the database. 
- Database: Stores multimedia content. 

This structure facilitates the data flow from the database to the end-user and back. 

## Why document software architectures? 

### Reflection questions
- Is a software architecture built to last instead of built to change? 
- Are the elements of a software architecture useful for a single application? 
- Are software architects oracles? If they can't see at least ten years ahead don't call them architects.
- Are software architectures only for software architects? 











