# Dockerfile

Blueprint how I want that container to be built and set up.

```
FROM node:latest

COPY . /src

WORKDIR /src

RUN npm install --production

EXPOSE 3000

CMD npm start

```

> copy everything from current directory into the containers ```src``` directory

> Work Directory: All the commands that I run, are going to be run inside of the /src

> EXPOSE 3000: This container exposes that port, so other containers can communicate with that container

> CMD: So I don't specify everytime I start that container what command to run


