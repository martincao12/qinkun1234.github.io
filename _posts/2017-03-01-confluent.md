---
layout: single
title: confluent
---

### How to Build a Scalable ETL Pipline with Kafka Connect

	$ ./start.sh
	
	mysql -u root --password="mypassword"

Using Kafka Connect to Ingest Data
	
	$ connect-standalone /mnt/etc/connect-avro-standalone.properties \
    /mnt/etc/mysql.properties /mnt/etc/hdfs.properties &


#### log

	/mnt/logs/hadoop-vagrant-namenode-ubuntu.out