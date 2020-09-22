FROM node:12.18.4-alpine3.9 AS CLIENT

LABEL maintainer="Luka Thuita <lthuita@gmail.com>"

WORKDIR /client
COPY . .  
RUN npm install
RUN npm run build
RUN npm install -g serve

EXPOSE 3000
CMD ["serve","-s", "build", "-l", "3000"]
