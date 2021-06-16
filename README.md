# hello-world-dotnet

A "hello world" application written in .NET Core.

## Running the Application

From the `hello-world-dotnet` subdirectory, run:

```bash
$ dotnet run
```

### Docker

From the `hello-world-dotnet` subdirectory, run:

```bash
$ docker build . -t hello-world-dotnet:latest
$ docker run -it --rm -e ASPNETCORE_URLS=http://+:5000 -e ASPNETCORE_ENVIRONMENT=Development -p 5000:5000 hello-world-dotnet:latest
```

### Docker Compose

From the `hello-world-dotnet` subdirectory, run:

```bash
$ docker-compose up --build
```

## Using the Application

This application serves a simple JSON payload at the root directory:

```bash
$ curl http://localhost:5000
```
