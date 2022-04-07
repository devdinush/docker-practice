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
docker run --name nodejs-hello-world-app -p 3000:3000 nodejs-hello-world-app:v1
```

#### Test:

```
localhost:3000
```
