# Project: Dockerizing a Python Flask Bookstore API with MySQL on AWS EC2 Using Terraform

## Description

The Bookstore Web API Application project aims to create a scalable bookstore web service using Docker and Terraform, providing students with an understanding of dockerizing applications and deploying them on AWS. The application, built with Python Flask, is deployed as a RESTful web service using Dockerfile and Docker Compose on an AWS EC2 instance using Terraform.

## Problem Statement

- Your team has initiated a project to create a Bookstore Web Service. Software developers have already built the first version of the application with the following database design:  

  - book_id: unique identifier for books, type is numeric.

  - title: title of the book, type is string.

  - author: author of the book. type is string.

  - is_sold: book availability status, type is boolean.

- They have also developed the RESTful web service using Python Flask. The table below outlines the HTTP methods for the resources identified by URIs:

| HTTP Method  | Action | Example|
| --- | --- | --- |
| `GET`     |   Obtain information about a resource | http://[ec2-hostname]/books|
| `GET`     |   Obtain information about a resource | http://[ec2-hostname]/books/123|
| `POST`    |   Create a new resource               | http://[ec2-hostname]/books|
| `PUT`     |   Update a resource                   | http://[ec2-hostname]/books/123 |
| `DELETE`  |   Delete a resource                   | http://[ec2-hostname]/books/123|

- As a cloud engineer, you are tasked with deploying the application in a development environment on a Docker Machine on AWS EC2 using Terraform. Your tasks include:

  - Fetching the application code from the GitHub repository.

  - Creating a Docker image using the `Dockerfile`.

  - Deploying the application using `docker compose`. Including;

    - Setting up a MySQL database service.

    - Configuring the application service to run on port 80.

    - Using a custom network for the services.

- The Terraform configuration should include:

  - Creation of new AWS resources for the application.

  - Running the application on an Amazon Linux 2 EC2 Instance.
  
  - Configuring the EC2 Instance as `t2.micro`.

  - Tagging the instance as `Web Server of Bookstore`

  - Ensuring the application is accessible via a web browser from anywhere.

  - Downloading the application files from the GitHub repo and deploying them on the EC2 Instance using a user data script within the Terraform configuration.

  - Outputting the Bookstore Web API URL after resource creation.

## Project Skeleton

```text
Bookstore Web API Application (Python Flask) with MySQL using Docker and Terraform on AWS (folder)
|
|----readme.md          # Given to the students (Definition of the project)
|----bookstore-api.py   # Given to the students (Python Flask Web API)
|----requirements.txt   # Given to the students (List of Flask modules for Web API)
|----main.tf            # To be delivered by students (Terraform config file)
|----docker-compose.yml # To be delivered by students
|----Dockerfile         # To be delivered by students
|----cfn-template.yml   # To be delivered by students (Optional)
```

## Expected Outcome

### Topics Covered;

- MySQL Database Configuration

- Bash scripting

- Docker Images

- Docker Compose

- AWS EC2 Service

- AWS Security Group Configuration

- AWS Cloudformation Service (Optional)

- Terraform Configuration with AWS

- Git & Github for Version Control System

### Skills Developed;

- Configuring MySQL database connections.

- Building Docker images.

- Configuring Docker Compose to run a Python Flask app.

- Improving bash scripting skills for application setup on EC2 Instances using Terraform.

- Configuring AWS EC2 Instances and Security Groups.

- Writing Terraform files to manage AWS resources.

- Using git commands and GitHub for version control.

- Deploying web applications on AWS EC2 using GitHub as a codebase.

## Steps to Solution
  
- Step 1: Clone the project definition from the `F3525-Ice` repo on Github

- Step 2: Create project folder for local public repo on your pc

- Step 3: Prepare scripts to build a Python Flask App Image using Dockerfile and Docker Compose

- Step 4: Prepare a Terrform configuration file to deploy your app on EC2 Instance

- Step 5: Push your application into your own public repo on Github

- Step 6: Deploy your application on AWS Cloud using Terraform to showcase your app within your team.

## Notes

- Use curl commands to showcase the REST functions for each HTTP method: GET, POST, PUT, DELETE.

## Resources

- [REpresentational State Transfer](https://en.wikipedia.org/wiki/Representational_state_transfer)

- [Terraform AWS Provider Documentaion](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)

- [AWS Cloudformation User Guide](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html) (Optional)
