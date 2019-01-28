FROM nodered/node-red-docker:rpi-v8

# installing an editor
USER root
RUN apt-get update && apt-get install nano
USER node-red

#RUN npm install node-red-contrib-resinio
#RUN npm install node-red-dashboard
#RUN npm install node-red-contrib-credentials
#RUN npm install node-red-contrib-os
#RUN npm install node-red-node-rbe
# RUN npm install node-red-contrib-influxdb
# RUN npm install node-red-contrib-fsm
# RUN npm install node-red-contrib-timerswitch
# RUN npm install node-red-contrib-mytimeout
# RUN npm install node-red-node-smooth
# RUN npm install node-red-contrib-bme280
# RUN npm install node-red-contrib-kalman
# RUN npm install node-red-contrib-esplogin

# COPY ./settings.js /data/settings.js
# COPY ./flows.json /data/flows.json
# COPY ./flows_cred.json /data/flows_cred.json
