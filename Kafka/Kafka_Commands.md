# Kafka Commands

---

### INICIANDO KAFKA:
**Zookeper:**
bin/zookeeper-server-start.sh config/zookeeper.properties 

**Kafka:**
bin/kafka-server-start.sh config/server.properties 

---

**DESCRIBRE:**
bin/kafka-topics.sh --bootstrap-server localhost:9092 --describe

---

**CREATE TOPIC:**
bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic LOJA_NOVO_PEDIDO

---

**CHANGE TOPIC (alterando para 3 partitions):**
bin/kafka-topics.sh --alter --topic ECOMMERCE_NEW_ORDER --bootstrap-server localhost:9092 --partitions 3

---

**DELETAR TOPIC:**
bin/kafka-topics.sh --bootstrap-server localhost:9092 --delete --topic __consumer_offsets

---
