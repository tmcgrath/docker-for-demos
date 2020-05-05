# Creates a 3 Broker Kafka cluster with Confluent

For demo purposes only... only runs one instance of Zookeeper.

The Brokers are available externally on mapped ports 19092, 29092 and 39092

Schema Registry is deployed as well.

## Requirements

1. Docker

2. Docker Compose

3. A solid, let's have a good time attitude

Hey, I'm no Docker expert by any means, so let me know if you see ways to improve.

## Steps

1. docker-compose up -d

## External Verification

1. kafka-topics --list --bootstrap-server localhost:29092

or 

2. if you have `kafkacat`, you cand do something like this `kafkacat -b localhost:19092 -L`

These commands from a terminal should verify you can access the Kafka cluster from outside of Docker containers themselves.
