# Workflow for running this project:


## Jenkins
- Created a jenkins container using Dockerfile in Jenkins folder, installed the required plugins and set username and password for admin user.
- Jenkins container runs on `localhost:3000`
- This Jenkins container have access to docker socket of host OS, it can control the docker containers and images of host using the same docker commands. For this, I used `-v /var/run/docker.sock:/var/run/docker.sock` flag in docker run command during container launch.

## Spring-Boot App.
- Created a simple 'hello world' app on java for the first time by following tutorials online.
- Created `Dockerfile` to create image using the `.jar` file of the project.
- After every change in the code , run `mvn clean install` and push the changes to github.





