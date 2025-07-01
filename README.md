# TodoApp HTML - Docker Instructions

This project contains a simple HTML Todo application.  
Follow the steps below to build, tag, and push the Docker image to Docker Hub.

---

## Build

```bash
docker build -t todoapp_html .
````

After building, you can verify the image exists:

```bash
docker images
```

---

## Login to Docker Registry

```bash
docker login
```

You'll be prompted to enter your Docker Hub username and password.

---

## Tag the Image

Tag your image with your Docker Hub username before pushing:

```bash
docker tag todoapp_html <your-dockerhub-username>/todoapp_html
```

Example:

```bash
docker tag todoapp_html tahs/todoapp_html
```

---

## Push to Docker Hub

```bash
docker push <your-dockerhub-username>/todoapp_html
```

Example:

```bash
docker push tahs/todoapp_html
```

---

## Summary

| Step  | Command Example                             |
| ----- | ------------------------------------------- |
| Build | `docker build -t todoapp_html .`            |
| Check | `docker images`                             |
| Login | `docker login`                              |
| Tag   | `docker tag todoapp_html tahs/todoapp_html` |
| Push  | `docker push tahs/todoapp_html`             |

---

