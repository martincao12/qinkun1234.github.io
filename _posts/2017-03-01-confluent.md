---
layout: single
title: How to Build a Scalable ETL Pipline with Kafka Connect
---

### command

	$ ./start.sh

	mysql -u root --password="mypassword"

Using Kafka Connect to Ingest Data

	$ connect-standalone /mnt/etc/connect-avro-standalone.properties \
    /mnt/etc/mysql.properties /mnt/etc/hdfs.properties &


#### log

	/mnt/logs/hadoop-vagrant-namenode-ubuntu.out

[How to Build a Scalable ETL Pipline with Kafka Connect](https://www.confluent.io/blog/how-to-build-a-scalable-etl-pipeline-with-kafka-connect/)
