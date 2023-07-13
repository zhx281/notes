# Create Dockerfile without Docker Compose

By creating a Dockerfile in root of the working directory will allow to fast build the image.

```
FROM python:3.10-slim

# set the working directory
WORKDIR /code

# install dependencies
COPY ./requirements.txt ./
RUN pip install --no-cache-dir --upgrade -r requirements.txt

# copy the src to the folder
COPY ./src ./src

# start the server
CMD ["uvicorn", "src.main:app", "--host", "0.0.0.0", "--port", "80", "--reload"]

```

# Create Docker Image with command line

```
docker build -t fastapi-image . 
```

- fastapi is the name
- . is the current work directory

# Run Docker Image as Container

```
docker run --name fastapi-container -p 80:80 -d -v $(pwd):/code fastapi-image
```

- --name specifi a name
- -p 80:80 map the port 
- -d run in deatch mode
- -v $(pwd):/code use volume to map the current working directory to /code in the container
- in powershell replace () with {}, -v ${pwd}:/code

# Stop and Remove container

```
docker stop fastapi-container
docker rm fastapi-contanier
```

- fastapi-container is just the name given to when create container, 
- when there is not name given during creation, docker will generate a random name

You could also uses the container id by listing all container with `docker ps -a` (-a or --all will show all cotnainer) and copying the id.

---

# Create dev enironment and share

### Dockerfile
1. Create Dockerfile file in the root project directory
2. add the codes
```
FROM python:3.10-slim
WORKDIR /code
COPY ./requirements.txt ./
RUN pip install --no-cache-dir --upgrade -r requirements.txt
COPY ./src ./src
CMD ["uvicorn", "src.main:app", "--host", "0.0.0.0", "--port", "80", "--reload"]
```


### docker-compose.yaml

1. Create a docker-compose.yaml file in the root project directory
2. add the codes
```
services:
  app:
    build: .
    command: uvicorn src.main:app --host 0.0.0.0 --port 80 --reload
    ports:
      - 80:80
    volumes:
      - .:/code
```
3. run `docker-compose up` in the terminal 
4. close the docker properly with `docker-compose down` after stoping the container
5. Rebuild with `--build` flag
6. add `-d` for deatch mode

---

# Using IDE

## VSCode

- install the docker and dev container extentions
- using the open remote connection button at bottem left to connect to the runing container
- select attach to container and the container enviornment

---

# Run docker cmd without sudo (linux)

1. Add docker to group
  - `sudo groupadd docker`
2. Add $USER to docker
  - `sudo gpasswd -a $USER docker`
  - note: Replace `$user` with the username of desire
3. Reboot `sudo reboot`
