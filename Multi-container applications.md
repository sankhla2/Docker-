1. Docker Compass
 we must start each container individually. Imagine how great it would be if a tool could start multiple containers with a single command. That tool is Docker Compose.

2. Sample application
   ``` bash
   git clone https://github.com/docker/multi-container-app

   ```
3. undestand the sample
This is a simple todo application built using ExpressJS and Node. All todos are saved in a MongoDB database.
<img width="385" alt="Screenshot 2024-09-07 at 1 19 47 AM" src="https://github.com/user-attachments/assets/0d6f3829-8967-4722-9bcf-6d60cb84325f">

4. If you view the code of the sample application, you will notice that it has a compose.yaml file. This file tells Docker how to run your application. Open the compose.yaml file in a text editor to explore the instructions.
5. Running the application
   We are going to run this application with the docker compose up command in your project directory. This command builds and runs all the services listed in the compose file.
``` bash
docker compose up -d
``` 
Breaking down the command
The -d flag tells docker compose to run in detached mode.
When developing with Docker, you may need to automatically update and preview your running services as you edit and save your code. We use docker compose watch for this.

Run the following command to run your project with compose watch.
``` bash
docker compose watch
```
Now change the text in line 18 of the app app/views/todos.ejs to see your changes in real time.

Read more about how to set this up in your own applications via the compose watch documentation⁠.

Stop watch mode

You can stop watch with Control (⌃)+ C shortcut.

