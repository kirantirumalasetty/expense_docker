FROM node:20
EXPOSE 8080
ENV DB_HOST="localhost"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY /schema/package.json .
COPY /schema/*.js .
RUN npm install
CMD [ "node", "index.js" ]