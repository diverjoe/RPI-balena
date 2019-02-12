FROM nodered/node-red-docker:rpi-v8

# installing an editor
USER root
RUN apt-get update && apt-get install nano 
USER node-red

#RUN echo "node-red ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers

RUN npm install node-red-contrib-resinio
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-credentials
RUN npm install node-red-contrib-os
RUN npm install node-red-node-rbe
RUN npm install node-red-contrib-influxdb
RUN npm install node-red-contrib-fsm
RUN npm install node-red-contrib-timerswitch
RUN npm install node-red-contrib-mytimeout
RUN npm install node-red-node-smooth
RUN npm install node-red-contrib-bme280
RUN npm install node-red-contrib-esplogin
RUN npm install node-red-contrib-i2c
RUN npm install node-red-contrib-interval-length
RUN npm install node-red-contrib-curve

COPY ./settings.js /data/settings.js
#COPY ./flows.json /data/flows.json
#COPY ./flows_cred.json /data/flows_cred.json

# see https://www.balena.io/docs/learn/develop/hardware/i2c-and-spi/
# following command changes the line in package.json :
#    "start": "node $NODE_OPTIONS node_modules/node-red/red.js -v $FLOWS"
# into
#    "start": "modprobe i2c-dev && node $NODE_OPTIONS node_modules/node-red/red.js -v $FLOWS"
#RUN sed -i  -e 's/node \$NODE_OPTIONS/modprobe i2c-dev \&\& node $NODE_OPTIONS/' package.json
