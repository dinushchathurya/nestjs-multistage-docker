## NestJs Multistage Docker


### Build Dev Docker Image

```
docker build -t nestmultistage-base -f Dockerfile-dev ./
```

### Build Prod Docker Image

```
docker build -t nestmultistage-prod -f Dockerfile-prod ./
```

### Build Actual Docker Image
```
docker build -t nest-multistage-service .
```

### Run Docker Container

```
docker run -p 3000:3000 --name nest-multistage nest-multistage-service
```

### Stop Running Container
```
docker stop nest-multistage
```

### Remove Container
```
docker rm nest-multistage
```

### Build Actual Docker Image Again
```
docker build -t nest-multistage-service .
```

### Run Docker Container

```
docker run -p 3000:3000 --name nest-multistage nest-multistage-service
```