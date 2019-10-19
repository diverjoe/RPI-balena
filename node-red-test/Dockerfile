FROM nodered/node-red:latest

# installing an editor
#USER root
#RUN apt-get update && apt-get install nano
USER node-red

RUN npm install node-red-contrib-resinio
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-credentials

COPY ./settings.js /data/settings.js
