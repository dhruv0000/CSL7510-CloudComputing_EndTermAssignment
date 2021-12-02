# Tick Stack
Telegraf, InfluxDB, Chronograf, and Kapacitor together make the TICK stack. The stack is generally used to make collecting, storage, graphing and alerting on a time series data set easy and convenient.
Telegraf: Collects and send metrics to InfluxDB. Has matrics collection support for 100+ services, using plugins.
InfluxDB: Used to store and access time-series data.
Chronograf: UI layer responsible for showing GRaphs and dashboards from InfluxDB and hook up alerts.
Kapacitor: Processing the metrics to look for an event and alerting the user using Chronograf.

We are going to run each stack in different containers, create a separate docker network for the containers to communicate in and bandle it all together in a docker-compose for easy deployment and sharing.

## Running the Code
```bash
cd tick.dockerapp
docker-compose up -d
```