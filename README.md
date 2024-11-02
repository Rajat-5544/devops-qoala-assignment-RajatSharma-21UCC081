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

Docker-Nginx-Logs

![](/screenshots/docker-nginx-logs.png)

---

## Steps

### 1. Initial Setup
1. **Clone the GitHub Repository:**
   - Start by cloning the provided GitHub repository, which contains the `Dockerfiles`, `docker-compose.yml` file, and the application code.
   
2. **Build Docker Images:**
   - Build each Docker image locally using the provided Dockerfiles.
   - Tag each image appropriately to be referenced by the `docker-compose.yml` file.

### 2. Running the Docker Compose File
1. **Start the Containers:**
   - Use the provided `docker-compose.yml` file to launch all containers.
   - **Note:** There are intentional errors in the code. Part of your assignment is to identify and fix these errors so the application runs correctly.

### 3. Debugging and Testing
1. **Identify Issues:**
   - Check the logs for any errors while building and running containers.
   - Examine the application code, Dockerfiles, and `docker-compose.yml` file to identify intentional errors.

2. **Resolve Errors:**
   - Document the issues and explain your debugging steps.
   - Apply necessary changes to the code, Dockerfiles, or configuration to resolve these errors.

3. **Verify Website Access:**
   - Open a web browser and access the application on `http://localhost` (or `http://<server-IP>` if hosted on a cloud server) to confirm it is running correctly.
   - Check Nginx or other web server logs to confirm requests are being logged as expected.

### 4. Submitting the Assignment
1. **GitHub Repository:**
   - Create a new GitHub repository and name it in this format: `devops-qoala-assignment-<name>-<rollnumber>`.
   - Upload all relevant files (including the modified code, Dockerfiles, `docker-compose.yml`, and other configurations) to this repository.
   - Grant access to `devops@qoala.id`. **Note:** Submissions without access granted will not be considered.

2. **Screenshots:**
   - Take a screenshot of the application running in the browser.
   - Include a screenshot showing Nginx (or web server) access logs that confirm a successful request.

3. **Report:**
   - Write a concise, one-page report that includes:
     - **Issues Identified:** Summarize any errors encountered during image building, container setup, or application testing.
     - **Resolution Steps:** Describe each action taken to resolve the issues and ensure the application runs correctly.

---

## Bonus Points

### Cloud Deployment
- For extra credit, deploy the application on a cloud server (AWS, GCP, or Azure) and provide an accessible endpoint, such as an IP address or DNS record.
- This will allow your work to be verified through the shared endpoint.

---

## Summary Checklist
- Set up Docker and Docker Compose.
- Clone and build Docker images.
- Debug and fix issues in code, Dockerfiles, or `docker-compose.yml`.
- Start containers and verify application accessibility on port 80.
- Upload files to a new GitHub repository and grant access to `devops@qoala.id`.
- Submit screenshots and a concise report of issues and solutions.
- (Bonus) Deploy on a cloud provider and share endpoint details.

---

Good luck, and happy debugging!
