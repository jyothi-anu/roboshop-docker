FROM node:20
WORKDIR /app
COPY *.json /app \
    server.js /app/
RUN npm install
ENV MONGO=true \
    MONGO_URL="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
CMD [ "/bin/node/app","server.js" ]