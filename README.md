# cnj-persistence-sql-downstream

Cloud native Java application based on Spring Boot acting as downstream service consumed by the other backends.

## Status

![Build Status](https://codebuild.eu-west-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiRTU3OVUwbzA1WmM5RExHYitjYlNla0lpam1BZDBaMkNuUWx0M2ZHYncvZnYyemtPM05iMC9tU1F0akMxZHdNQ0NZMHhyZmxwOXZiT3FFY0JaaURFc0tVPSIsIml2UGFyYW1ldGVyU3BlYyI6Ind6Zk4wUGUya3JIYnp0Ly8iLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

## Release information

Check [changelog](changelog.md) for latest version and release information.

## Docker Pull Command

`docker pull docker.cloudtrain.aws.msgoat.eu/cloudtrain/cnj-persistence-sql-downstream`

## HOW-TO build this application locally

If all prerequisites are met, just run the following Maven command in the project folder:

```shell 
mvn clean verify -P pre-commit-stage
```

Build results: a Docker image containing the showcase application.

## HOW-TO start and stop this showcase locally

In order to run the whole showcase locally, just run the following docker commands in the project folder:

```shell 
docker compose up -d
docker compose logs -f 
```

Press `Ctlr+c` to stop tailing the container logs and run the following docker command to stop the showcase:

```shell 
docker compose down
```

## HOW-TO demo this showcase

The showcase application will be accessible:
* locally via `http://localhost:38080`
* remotely via `https://train2023-dev.k8s.cloudtrain.aws.msgoat.eu/cloudtrain/cnj-persistence-sql-downstream` (if the training cluster is up and running)

The OpenAPI specification of the exposed REST API is available at URI `/openapi`.
