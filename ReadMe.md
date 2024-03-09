# Web Server in Docker
This repository contains a Dockerfile to build a custom web server image.

![System Architecture Diagram](https://github.com/aakashgoel2002/Docker-Web-Server/blob/main/SA-Diagram.png?raw=true)
<img src="https://github.com/aakashgoel2002/Docker-Web-Server/blob/main/SA-Diagram.png" alt="System Architecture Diagram" style="width:250px;"/>


### Building the Image
To build the image, run the following command from the root directory of this repository:

```bash
docker build -t my-web-server .
```

This will build an image with the tag `my-web-server`.

### Running the Container
To run the container, use the following command:

```bash
docker run -d -p 80:80 my-web-server
```

This will start a new container in the background, mapping port 80 inside the container to port 80 on the host machine.

### Stopping the Container
To stop the container, run the following command:

```bash
docker stop my-web-server
```

Replace `my-web-server` with the name of your container if it is different.

### Removing the Container
To remove the container, use the following command:

```bash
docker rm my-web-server
```

Replace `my-web-server` with the name of your container if it is different.

### Removing the Image
To remove the image, use the following command:

```bash
docker rmi my-web-server
```
Replace `my-web-server` with the name of your image if it is different.

### Dockerfile
The `Dockerfile` in this repository contains instructions to build a simple web server using the apache. It copies a custom `index.html` file to the container and starts the `apache` service.

Feel free to modify the `Dockerfile` and `index.html` file to suit your needs.

