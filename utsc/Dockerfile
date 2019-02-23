FROM nodered/node-red-docker:rpi-v8

# installing an editor
USER root
RUN apt-get update && apt-get install nano
USER node-red

RUN npm install node-red-contrib-resinio
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-credentials


COPY ./flows.json /data/node-red/flows.json
COPY ./flows_cred.json /data/node-red/flows_cred.json
COPY ./settings.js /data/node-red/settings.js
