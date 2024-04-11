# Kafka Python Getting Started

This is based on tutorial https://developer.confluent.io/get-started/python

```shell
virtualenv env

source env/bin/activate

pip install confluent-kafka

confluent local kafka start
```

Update `getting_started.ini` with the Plaintext Ports output from last command.

```shell
chmod u+x producer.py

./producer.py getting_started.ini
```

```shell
chmod u+x consumer.py

./consumer.py getting_started.ini
```

```shell
confluent local kafka stop
```

```shell
deactivate
```