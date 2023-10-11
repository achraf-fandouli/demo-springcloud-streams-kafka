# demo-springcloud-streams-kafka
pour démarrer :
1- Télécharger broker kafka(kafka download).
2- Démarrer zookeeper (dans le dossier bin lancer la ligne de commande):
start zookeeper-server-start.bat D:\projects\Kafka\kafka_2.13-2.7.0\config\zookeeper.properties

3- Démarrer serveur kafka (dans le dossier bin lancer la ligne de commande) :
start kafka-server-start.bat D:\projects\Kafka\kafka_2.13-2.7.0\config\server.properties

Par la suite il y a deux clients kafka qu’on peut les utiliser pour faire quelque test :

Kafka console producer
Kafka console consumer
Kafka se trouve par défaut sur le port : 9092. Pour les démarrer :

Dans le dossier ben puis windows, exécutez les commandes suivantes :

4- Lancer un consommateur kafka pour attendre les messages arrivant sur le sujet R1 : kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic R1

5- Lancer le client kafka producer : kafka-console-producer.bat --broker-list localhost:9092 --topic R1

En fin, si nous créons un message test au niveau du producer, le consommateur recevra le message test ;
