# Builds a docker image running Kafka MongoDB Connector.
# Needs to be linked with kafka and schema-registry containers.
# Usage:
#   docker build -t teambition/kafka-connect-mongo kafka-connect-mongo
#   docker run -d --name kafka-connect-mongo --link kafka:kafka --link schema-registry:schema-registry teambition/kafka-connect-mongo

FROM confluentinc/cp-kafka-connect-base:3.2.1

MAINTAINER sailxjx@gmail.com

COPY targets "/usr/local/kafka-connect-mongo/"
RUN ln -sf /usr/local/kafka-connect-mongo/lib /usr/share/java/kafka-connect-mongo
