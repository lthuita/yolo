FROM node:12.18.4-alpine3.9 AS CLIENT

LABEL maintainer="Luka Thuita <lthuita@gmail.com>"
LABEL description="this is for the frontend container"


WORKDIR /client
COPY . .  
RUN npm install
RUN npm run build
RUN npm install -g serve

EXPOSE 3000
CMD ["serve","-s", "build", "-l", "3000"]


# the built image was also pushed to the docker hub - https://hub.docker.com/repository/docker/lthuita/yolo_frontend
