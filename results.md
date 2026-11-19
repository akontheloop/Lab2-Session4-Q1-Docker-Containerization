# Practical Results

## 1. Docker Image
The `sample-app` image was built successfully using the Dockerfile.

## 2. Container
The container named `myapp` was created and run with port 8000 mapped to the host.

## 3. Application Test
Command:
```bash
curl http://localhost:8000
```
Response:
```html
<h1>Hello from Docker Container!</h1>
```

## 4. Logs
`docker logs myapp` was used to view the application logs.

## 5. Container Stop and Restart
The container was stopped using `docker stop myapp`, checked using `docker ps`, and restarted using `docker start myapp`. The application was tested again successfully.

## 6. Image Layers
`docker history sample-app` was used to display the image's layer history. `docker image inspect sample-app` was used to inspect image metadata.

## Conclusion
The sample Python web application was successfully containerized, built into a Docker image, run in a container, tested, stopped, restarted, and inspected.
