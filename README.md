## In MAC

sudo chmod 600 ~/.ssh/Nono29.pem

ssh -i ~/.ssh/Nono29.pem ubuntu@54.92.212.195


## In UBUNTU

sudo apt-get update

sudo apt-get install git

git clone https://github.com/NoraArouchian/Nora-s-Repository.git

sudo useradd kafka -m

sudo passwd kafka

sudo adduser kafka sudo

su - kafka

## In KAFKA

sudo apt-get update

sudo apt-get install default-jre

sudo apt-get install zookeeperd

telnet localhost 2181

mkdir -p ~/Downloads

wget "http://mirror.bit.edu.cn/apache/kafka/1.0.0/kafka_2.11-1.0.0.tgz" -O ~/Downloads/kafka.tgz

## In KAFKA

mkdir -p ~/kafka && cd ~/kafka

tar -xvzf ~/Downloads/kafka.tgz --strip 1

nano ~/kafka/config/server.properties

nohup ~/kafka/bin/kafka-server-start.sh ~/kafka/config/server.properties > ~/kafka/kafka.log 2>&1 &

bin/kafka-server-start.sh config/server.properties

export KAFKA_HEAP_OPTS="-Xmx256M -Xms128M"

bin/kafka-server-start.sh config/server.properties

## In Another Terminal KAFKA

su - kafka

cd ~/kafka

bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Nora

bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Nora


## In Another Terminal KAFKA

su - kafka

cd ~/kafka

bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic Nora --from-beginning


nano ~/.bash_history
