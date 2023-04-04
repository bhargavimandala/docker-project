# base image for node js
FROM node:14
# expose the appliaction 
EXPOSE 8080
# It is used to set the path to the image and container while creating
WORKDIR /opt/server
#copy files from local to container
COPY package.json /opt/server/
# run install packages, softwares
RUN npm install
COPY server.js /opt/server/
#It will run the container
ENTRYPOINT ["node", "server.js"]

