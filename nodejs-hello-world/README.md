#### To Build the Docker image:

```
docker build -t IMAGE_NAME:TAG_NAME .
```

```
docker build -t nodejs-hello-world-app:v1 .
```

#### To run the image:

```
docker run -p HOST_PORT:CONTAINER_PORT -d IMAGE_NAME:TAG_NAME
```

```
docker run --name node-hello-world-app -p 8080:8080 node-hello-world-app:v1
```

#### Test
Check browser: localhost:3000
