FROM node:latest

# Command COPY is not needed because in docker-compose.yaml it is using command 'volumes'
# COPY . .

RUN apt update && \
    apt install -y wget netcat-traditional && \
    wget -q -O /usr/bin/wait-for https://raw.githubusercontent.com/eficode/wait-for/v2.2.3/wait-for && \
    chmod +x /usr/bin/wait-for

USER node

WORKDIR /usr/src/app
EXPOSE 3000

# Uncomment to use without dockerize
# CMD [ "node", "index.js" ]
# docker build -t barbiericontainer/app-node-with-mysql-and-nginx .
# docker run -d -p 3000:3000 barbiericontainer/app-node-with-mysql-and-nginx:latest