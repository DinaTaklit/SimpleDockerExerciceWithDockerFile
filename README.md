# SimpleDockerExerciceWithDockerFile

## Run the exercice

- Build the image from the same directory using the command
  
```bash
docker build -t test .
```

>Note that the full stop . tells the docker build command using the Dockerfile found in the current directory.

>Here, the -t flag is an alternate way of writing `--tag`

- Run the container with the following command:

```bash
docker run  -p 80:8080 test
```

> In this command, you are binding port 8080 of the container to the port 80 of your local machine. The flask application

- When you are finished, get the id of the running container:
  
```bash
docker ps
```

- You can then use the id to stop the container:
  
```bash
docker stop <Container Id>
```