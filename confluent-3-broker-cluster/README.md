# Creates a 3 Broker Kafka cluster with Confluent images

For demo purposes only... only runs one instance of Zookeeper.

The Brokers are available externally on mapped ports 19092, 29092 and 39092

## Requirements

1. Docker

2. Docker Compose

3. A solid, let's have a good time attitude


## Steps

1. docker-compose up -d

## Verification

1. kafka-topics --list --bootstrap-server localhost:29092

or 

2. if you have `kafkacat`, you cand do something like this `kafkacat -b localhost:19092 -L`


