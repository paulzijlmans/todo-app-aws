# Todo app

The first version of the Todo app contains only a static page. We're using this app to demonstrate how to deploy a Spring Boot application to AWS.

Resource: Stratospheric - From Zero to Production with Spring Boot and AWS (https://github.com/stratospheric-dev)

## Local

### Build
```./gradlew build```

### Run
```./gradlew bootrun```

Open your browser to `http://localhost:8080/`.

## Docker

### Build
```docker build -t pzijlmans/todo-app-v1:latest``` 

### Publish to Docker Hub
```docker login```

```docker push pzijlmans/todo-app-v1:latest```

### Pull the image from Docker Hub
```docker pull pzijlmans/todo-app-v1:latest```

## AWS

### Deploy application to AWS using CloudFormation
```cd cloudformation```

```./create.sh``` 

### Delete application from AWS using CloudFormation
```cd cloudformation```

```./delete.sh```