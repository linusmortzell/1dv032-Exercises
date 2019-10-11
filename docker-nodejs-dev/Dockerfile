FROM node

LABEL version="1.0"
LABEL maintainer="lm222qm"

RUN mkdir -p /opt/app 

WORKDIR /opt/app

COPY package.json .

RUN npm install --quiet

VOLUME /opt/app/node_modules

COPY . .

EXPOSE 8080

CMD ["npm", "start"]