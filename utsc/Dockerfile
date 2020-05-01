FROM nodered/node-red-docker
# installing an editor
USER root
RUN apt-get update && apt-get install nano
USER node-red

RUN npm install node-red-contrib-resinio
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-credentials
RUN npm install node-red-contrib-alexa-local
RUN npm install node-red-contrib-alexa-notifyme
RUN npm install node-red-contrib-bigtimer
RUN npm install node-red-contrib-collector
RUN npm install node-red-contrib-eztimer
RUN npm install node-red-contrib-fsm
RUN npm install node-red-contrib-home-assistant-websocket
RUN npm install node-red-contrib-influxdb
RUN npm install node-red-contrib-interval-length
RUN npm install node-red-contrib-match
RUN npm install node-red-contrib-moment
RUN npm install node-red-contrib-mytimeout
RUN npm install node-red-contrib-timerswitch
RUN npm install node-red-node-email
RUN npm install node-red-node-feedparser
RUN npm install node-red-node-rbe
RUN npm install node-red-node-sentiment
RUN npm install node-red-node-smooth
RUN npm install node-red-node-tail
RUN npm install node-red-node-twitter
RUN npm install node-red-node-ui-etable
RUN npm install node-red-node-ui-table

COPY ./settings.js /data/ae/settings.js
