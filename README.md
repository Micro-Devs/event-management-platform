# <p align="center"> Project Structure Images </p>

<p align="center"> 
  <a href="https://ibb.co/fXFd2RS"><img src="https://i.ibb.co/qDjYdGn/Whats-App-Image-2024-12-27-at-18-35-43.jpg" alt="Whats-App-Image-2024-12-27-at-18-35-43" border="0"></a>
</p>
<p align="center"> 
  <a href="https://ibb.co/dDrrdG6"><img src="https://i.ibb.co/FzKKSgJ/Whats-App-Image-2024-12-27-at-18-35-28.jpg" alt="Whats-App-Image-2024-12-27-at-18-35-28" border="0"></a>
</p>

## <p align="center"> Cloning Project to Local </p>

- <strong> Clone the main repository to your local. </strong>
```
git clone --recurse-submodules https://github.com/Micro-Devs/event-management-platform.git
```

<br/>

- <strong> Checkout to main for all submodules </strong>
```
git checkout main && git submodule foreach 'git checkout main'
```

<br/>

- <strong> Apply the commands below to update existing submodule. </strong>

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

<br/>

- <strong> To add a submodule </strong>

```
git submodule add https://github.com/Micro-Devs/[service-name].git services/[service-name]
```

<br/>

- <strong> To pull all submodules </strong>

```
git pull --recurse-submodules
```


## <p align="center"> Docker / Kafka Commands </p>
docker exec -it [Kafka_Container_ID] /bin/bash

new topic: kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions [Partition_Sayısı] --topic [Topic_Adı]

ex: kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic myTopic

get all topic list: kafka-topics.sh --list --bootstrap-server localhost:9092

## <p align="center"> Compose Commands </p>
docker-compose up -d