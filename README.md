# Lab 2 – Session 4 – Question 1
## Containerize a Sample Application Using Docker

### Objective
Create a sample Python web application, containerize it using Docker, build an image, run a container, and observe image layers and container behavior.

### Files
- `app.py` – Simple Python HTTP server returning an HTML response.
- `Dockerfile` – Instructions to build the Docker image.
- `commands.txt` – Commands used in the practical.
- `results.md` – Expected/observed demonstration results.

### Run the application
Build the image:
```bash
docker build -t sample-app .
```

Run the container:
```bash
docker run -d -p 8000:8000 --name myapp sample-app
```

Test:
```bash
curl http://localhost:8000
```

Open in browser: http://localhost:8000
