## <p align="center"> Cloning Project to Local </p> 

- <strong> Clone the main repository to your local. </strong>
```
git clone --recurse-submodules https://github.com/Micro-Devs/event-management-platform.git
```
<br/>

- <strong> Apply the commands below to update existing submodule. <strong>

```
git submodule init
```
```
git submodule update
```

<br/>

- <strong> First, go to the path of the submodule. </strong>
- <strong> Apply the commands below in order to pull the last changes of the related submodule. </strong>

```
git checkout dev
```
```
git pull
```


## <p align="center"> Docker / Kafka Commands </p>
docker exec -it [Kafka_Container_ID] /bin/bash

new topic: kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions [Partition_Sayısı] --topic [Topic_Adı]

ex: kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic myTopic

get all topic list: kafka-topics.sh --list --bootstrap-server localhost:9092

## <p align="center"> Compose Commands </p>
docker-compose up -d
