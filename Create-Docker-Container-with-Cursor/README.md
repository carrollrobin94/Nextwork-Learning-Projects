<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Create a Docker Container using Cursor

**Project Link:** [View Project](http://nextwork.ai/projects/ai-mcp-docker)

**Author:** Carroll Robin Shelby  
**Email:** carrollrobin94@gmail.com

---

---

## Introducing Today's Project!

In this project, I'm going to create and manage a PostgreSQL Database Container through natural language in Cursor AI and Docker MCP

### Key tools and concepts

The key tools I used include Docker Desktop and Cursor. Key concepts that I have learnt include Cursor helping me to create a PostgreSQL database container through natural language with keywords such as "Database name, map port, username and password" . However before using Cursor, first I had to establish the communication between Docker and Cursor by using MCP which was made possible by Python's uv extension. After creating the the database container, I needed a way to view the database visually and it was made possible by using Adminer, this set up was also done through Cursor and Docker Compose which made the two containers, Adminer and PostgreSQL , work together to produce a web page to view the database. Additionally, I learned that you can use Cursor to monitor and manage the logs from containers and take action upon them without any manual coding if any issues arises 

### Challenges and wins

This project took me approximately one and a half hour because setting up Docker and Cursor took some time and faced some simple errors such as the container not working and reaching the usage limits of Cursor

### Why I did this project

I did this project today to learn how to use Docker and Cursor as I am not familiar with the usage of Cursor than the other AI tools available online and also learn a bit about Docker, how it works and what can be done with it. MCP was entirely a new concept to me and I am glad that I have learned it since it can take some monitoring and managing works from the hands of the developers and be able to focus more on the architecture of the system

---

## Setting Up Cursor and Docker Desktop

In this step, I'm installing Cursor and Docker Desktop. I need Cursor because through natural language, it will create and manage the PostgreSQL database for a specific application and Docker Desktop will host the database within a container

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_8h9i0j1k)

### Why Docker containers?

Docker containers are useful because they can containerize apps with everything it needs into a lightweight bundle and also keep it isolated from other containers within Docker Desktop

---

## Connecting Cursor to Docker with MCP

In this step, I'm installing uv, a fast python package manager which helps with Docker and later enabling Docker MCP in Cursor to create the database through natural language 

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_8g9h0i1j)

### Installing Python and uv

To set up the Docker MCP, I installed Python to run the uv as it's used to establish the connection between Cursor and Docker Desktop through the MCP while running in the background 

### What the Docker MCP can do

The Docker MCP lets me list containers, get logs from containers, create a container from reference images,  deploy a Docker Compose or Docker Stack

---

## Creating My First PostgreSQL Container

In this step, I'm going to prompt the Cursor AI to create a PostgreSQL container and verify that the container is running in Docker by opening Docker Desktop

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_7k8m9n0p)

### Verifying the container

I verified my container by checking Docker Desktop where I can see the green dot and hovering over the green dot shows the status "Running" of the PostgreSQL database my-db

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_2q3r4s5t)

---

## Orchestrating Multiple Containers with Docker Compose

In this step, I'm setting up a project folder on my desktop and later using it to set up the PostgreSQL and Adminer with Docker Compose. Adminer helps us view the database visually through a single page in the web browser

### Setting up the docker-compose.yml file

The purpose of Docker Compose is to set up two containers that work together and it's all hosted in docker-compose.yml file. One of the container is the PostgreSQL database and the other is Adminer used to visualize the database. When both of them work together, a user can visually check the data in the database 

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_x7z1b4c6)

### Accessing the database in the browser

I verified my database by logging into Adminer at localhost:8081 where I can see the absolute path of the file "my-db" starting from the root directory of PostgreSQL » my-db » nextwork » Schema: public 

---

## Monitoring Container Logs

In this project extension, I'm going to check the container logs through Cursor AI and understand what log entries mean.

![Image](http://nextwork.ai/lively_orange_innocent_peacock/uploads/ai-mcp-docker_9y0z1a2b)

### What I learned from the logs

I checked my container logs without using Docker Desktop by first prompting Cursor to show me the logs for container "my-db" and later asked it to explain any issues or errors that may have occured and was recorded in the logs

---

---
