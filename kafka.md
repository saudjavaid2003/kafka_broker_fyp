### Create Kafka topic:

./kafka-topics.sh --create --topic product --bootstrap-server localhost:9092

List Kafka topics:

./kafka-topics.sh --list --bootstrap-server localhost:9092

Get Topic details, partition counts etc.
./kafka-topics.sh --describe --bootstrap-server localhost:9092 --topic product

Alter the topic, change partition:
./kafka-topics.sh --alter --bootstrap-server localhost:9092 --topic product --partitions 6

Publish a message to Kafka topic

./kafka-console-producer.sh --bootstrap-server localhost:9092 --topic pricing

Check messages in a topic
./kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic product --from-beginning


// ek kam mujay kerna ha ab 
dekho ek taraf ha order service dosri taraf ha kafka aur us say attach hain consumers notification or websockets service  ab ferx karo  kay kuch hoa aur consumers bend ho ghay to 
kuch dher bad dobara say wo start houn ghay ek ek ke rkay evnet lein ghay lekin order nai ho gha to key ko add karo her event kay orderId ko as a key
