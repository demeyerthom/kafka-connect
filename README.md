# Kafka Connect container and chart

## Environment variables
- `CLASSPATH`: The path where plugins are stored
- `CONNECT_BOOTSTRAP_SERVERS`: A list of host/port pairs to use for establishing the initial connection to the Kafka cluster
- `CONNECT_GROUP_ID`: A unique string that identifies the Connect cluster group this worker belongs to
- `CONNECT_CONFIG_STORAGE_TOPIC`: The name of the Kafka topic where connector configurations are stored
- `CONNECT_OFFSET_STORAGE_TOPIC`: The name of the Kafka topic where connector offsets are stored
- `CONNECT_STATUS_STORAGE_TOPIC`: The name of the Kafka topic where connector and task status are stored
- `CONNECT_KEY_CONVERTER`: Converter class used to convert between Kafka Connect format and the serialized form that is written to Kafka
- `CONNECT_VALUE_CONVERTER`: Converter class used to convert between Kafka Connect format and the serialized form that is written to Kafka
- `CONNECT_REST_ADVERTISED_HOST_NAME`: If this is set, this is the hostname that will be given out to other workers to connect to
- `CONNECT_REST_PORT`: Port for the REST API to listen on
- `CONNECT_KEY_CONVERTER`: Converter class used to convert between Kafka Connect format and the serialized form that is written to Kafka
- `CONNECT_KEY_CONVERTER_SCHEMA_REGISTRY_URL`
- `CONNECT_VALUE_CONVERTER`: Converter class used to convert between Kafka Connect format and the serialized form that is written to Kafka
- `CONNECT_VALUE_CONVERTER_SCHEMA_REGISTRY_URL`
- `KAFKA_JMX_OPTS`
- `KAFKA_JMX_HOSTNAME`

See https://kafka.apache.org/documentation/#connectconfigs. Any of these configs can be added by converting the config 
to upper case and underscore and adding `CONNECT_` as prefix.