# Mission Reflection

This laboratory helped me understand the practical difference between Virtual Machines and containers. When installing an operating system on a Virtual Machine, the process usually takes more time because the VM needs to create virtual hardware resources and boot a complete guest operating system. In comparison, a Docker container can start within seconds because it shares the host operating system kernel and only needs the required application and dependencies. This makes containers faster and more efficient for many modern applications.

Port mapping is necessary when running a web server inside a container because the application is isolated inside the container. The Nginx server listens on port 80 inside the container, but users outside the container need a way to access it. The command `-p 8080:80` connects port 8080 of the host machine to port 80 of the Nginx container. Because of this mapping, I can access the Nginx web server by using `http://localhost:8080`.

When the `docker rm` command is used, the specified container is permanently removed after it has been stopped. Any data stored only inside the writable layer of that container is also removed. This shows why important application data should normally be stored using persistent storage such as Docker volumes instead of relying only on the container itself.

Containerization also changes how developers and IT operations teams work together. Developers can package an application and its dependencies into a consistent container image, while operations teams can deploy the same image across different environments. This supports DevOps practices because it reduces environment differences and makes deployment more repeatable.

My GitHub portfolio is also evolving from simple cloud computing activities into a more organized technical portfolio. By documenting commands, screenshots, explanations, and reflections, I am building evidence of practical skills instead of only collecting theoretical information. This laboratory gave me experience with Docker, Linux, containers, networking, and technical documentation.

