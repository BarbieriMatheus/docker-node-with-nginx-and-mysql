FROM node:latest

WORKDIR /usr/src/app

# Command COPY is not needed because in docker-compose.yaml it is using command 'volumes'
# COPY . .

# RUN echo "deb http://archive.debian.org/debian stretch main" > /etc/apt/sources.list

# ENV DOCKERIZE_VERSION v0.7.0
# RUN apt-get update \
#     && apt-get install -y wget \
#     && wget -O - https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz | tar xzf - -C /usr/local/bin \
#     && apt-get autoremove -yqq --purge wget && rm -rf /var/lib/apt/lists/*


EXPOSE 3000

# Uncomment to use without dockerize
CMD [ "node", "index.js" ]
# docker build -t barbiericontainer/app-node-with-mysql-and-nginx .
# docker run -d -p 3000:3000 barbiericontainer/app-node-with-mysql-and-nginx:latest