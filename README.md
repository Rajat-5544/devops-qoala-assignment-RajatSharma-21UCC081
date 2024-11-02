# DevOps Assignment: Debugging and Running a Dockerized Application

This report documents the process of debugging and running a Dockerized application as part of a hiring assignment for Qoala.

## Debugging Process

I started with the Python folder. I identified and corrected typos in the Dockerfile. After doing this, I successfully created an image tagged qoala/python-app.

Continuing, I navigated into the Nginx folder; here I saw some typos in both the Dockerfile and also the nginx.conf that I corrected. At this, I had also added an HTML folder to the Nginx directory. Finally, after making these errors right, I built it and assigned the tag qoala/nginx.

Lastly, I debugged the docker-compose.yaml file with a number of typographical errors. Correcting those allowed me to run the application using the command: docker-compose up --build

Having successfully built the images, I accessed the application on localhost:80. The application responded as expected, thus showing that the setup and debugging processes were successful.

Bonus: Cloud Deployment
Bonus points I ran the application on AWS cloud server EC2. In this, I followed instructions for launching a new EC2 instance.The public IP address for accessing the application is at http://13.60.172.194/.

---

## Screenshots

**1**

AWS-Cloud-Deployment

![](/screenshots/awsdeployapp.png)

**2**

Running-On-Localhost:80 

![](/screenshots/localhostapp.png)

**3**

Docker-Nginx-Logs

![](/screenshots/docker-nginx-logs.png)

**4**

Docker-Python-App-Logs

![](/screenshots/docker-python-logs.png)

---

## What I Learned

1. **Understanding Docker:**
   I understood what Docker is, what it does, and how to use it most effectively.
   
2. **Docker Commands:**
   I became familiar with essential Docker commands and their applications.

3. **YAML:**
   In addition, I learned the basic idea of YAML- especially in connection with some files, such as docker-compose.yaml.

4. **Cloud Deployment:**
   I gained experience in deploying Dockerized applications on an AWS cloud server, enhancing my understanding of cloud infrastructure.
