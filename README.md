# SmartHome Project with Sonoff and Shelly devices works also with Amazon Echo.

The Project can run on a Raspberry Pi 4 (4GB). 

#### Node-RED:
Use the smartHome.json file to import all the configs into Node-RED. Project was made with Node-RED Version v.0.16.1

Node-RED Library used:

```
npm install node-red-contrib-amazon-echo
npm install node-red-dashboard
npm install node-red-contrib-re-postgres
npm install node-red-contrib-telegrambot
npm install node-red-contrib-interval-length
npm install node-red-contrib-time-range-switch
```

#### Eclipse Mosquitto:
Used to build mqtt broker connection to shelly devices and sonoff devices.

#### Portainer:
To maintain docker via a WebInterface.

#### NetData:
Used to get out a short summary of the performance of the host system.

#### Grafana/Telegraf/InfluxDb:
Used for monitoring of performance from host system and docker system.
Each docker Container can be monitored in detail.
Telegraf is writing the data into influxdb. From there Grafana is building the dashboards.

#### Telegram:
Important notifications will be sent out to a Telegram Bot. 

#### PostgreSQL
Used to store important data for history overview. Not included in this Git repository. Please check the node-red config and build a suitable environment if you like to use it.
