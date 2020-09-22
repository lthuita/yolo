FROM node:12.18.4-alpine3.9 AS BACKEND

LABEL maintainer="Luka Thuita <lthuita@gmail.com>"
LABEL description="this is for the backend container"

WORKDIR /backend
COPY . . 

RUN npm install

EXPOSE 5000
CMD [ "npm", "start" ]


# the built image was also pushed to the docker hub - https://hub.docker.com/repository/docker/lthuita/yolo_backend
