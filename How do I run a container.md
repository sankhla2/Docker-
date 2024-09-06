1. <img width="347" alt="Screenshot 2024-09-07 at 12 53 55 AM" src="https://github.com/user-attachments/assets/5b5713d8-1e5f-411f-baa3-97eecc712cc1">
2. Get a sample application
   Clone the repository at https://github.com/docker/welcome-to-docker⁠.
``` bash
git clone https://github.com/docker/welcome-to-docker
```
The rest of this guide requires you to run commands in the new project directory. Run the following command before moving on.
``` bash 
cd welcome-to-docker
```

3. verifying the Dockerfile
   Open the sample application in your IDE. Note that it already has a Dockerfile. For your own projects you need to create this yourself.
<img width="625" alt="Screenshot 2024-09-07 at 12 56 25 AM" src="https://github.com/user-attachments/assets/4e90596c-7317-4728-beab-697111cc9125">

4. Build your first image
You can build an image using the following docker build command via a CLI in your project folder.
``` bash
docker build -t welcome-to-docker .
```
Breaking down this command

The -t flag tags your image with a name. (welcome-to-docker in this case). And the . lets Docker know where it can find the Dockerfile.
# Welcome to Docker

This is a repo for new users getting started with Docker.

You can try it out using the following command.
```
docker run -d -p 8088:80 --name welcome-to-docker docker/welcome-to-docker
```
And open `http://localhost:8088` in your browser.

# Building

Maintainers should see [MAINTAINERS.md](MAINTAINERS.md).

Build and run:
```
docker build -t welcome-to-docker . 
docker run -d -p 8088:3000 --name welcome-to-docker welcome-to-docker
```
Open `http://localhost:8088` in your browser.



5. run your container
 Once the build is complete, an image will appear in the Images tab. Select the image name to see its details. Select Run to run it as a container. In the Optional settings remember to specify a port number (something like 8089).
