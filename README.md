# Running an Apache server on Docker

Using the official image of Httpd on Docker Hub, a personalized index.html file and a Dockerfile to combine the two, we can access a containerized Server on our machine by visiting  http://localhost:8080 .

## Usage

Create a new image based on the Dockerfile by executing the following command inside the directory in which the Dockerfile is located (for us is the Docker folder):
```
docker build -t my-apache2 . 
```

Next we run the image created:
```
docker run --name my-running-app -p 8080:80 -d my-apache2
```

Now everything should be good and running.
