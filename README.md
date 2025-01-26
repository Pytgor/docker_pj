 # Project Overview

This project is a simple web server using Node.js and NGINX. In this project, NGINX is used as a reverse proxy, forwarding all traffic to 3 instances of the same web application created using Docker Compose. The load balancing algorithm used is **Least Connections**.

## Requirements

- **NGINX** (installed on the host machine)
- **Docker** and **Docker Compose**

## How to Use

### 1. Install NGINX
a- Make sure NGINX is installed on your host machine as it will be used as the reverse proxy.
b- run npm install to install dependencies but make sure to be in the project directory
c- Start nginx by running  nginx 
d- run the docker-compose file by using  the next command ( docker-compose up -d ), after this make 
sure that the container are running by using docke ps -a and now to log in into the website and see if the container
working properly got to localhost:3001 localhost:3002 localhost:3003 to see if  the 3 instances of the app are working
e- Now test if SSL is working, just in case SSL is same as https (run this https://localhost)

### 2. Install Dependencies
Run the following command in the project directory to install the necessary dependencies:

```bash
npm install
