# IoT Aggregator

This is a project to create a basic kubernetes cluster for aggregating data from multiple IoT devices.

The cluster includes the following functionality:

1. MQTT Broker to receive and buffer data from IoT devices
2. A golang service to act as a pipeline from MQTT to Kafka for incoming data
3. Kafka to queue and route incoming data
4. a golang service to receive and persist incoming data<br/>
   *For now, we'll use a postgres db to store the raw data. This will likely change to something more appropriate such as a lake or warehouse*

