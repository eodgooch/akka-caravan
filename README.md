akka-caravan
=============

This project aims to use the Akka ActorSystem to read messages from Oracle ActiveQueue and write to Apache Kafka in a asynchronous, highly available, fault tolerant system. The project could easily be extended to use Apache Camel to send messages from Oracle ActiveQueue to any other system Camel integrates with.

Use a configuration file to start:

```javascript
	{
		"oracle" : {
			"jdbc_url" : "",
			"connection_pool_size" : 1,
			"num_consumers" : 5,
			"batch_size" : 100
		},
		"kafka" : {
			"broker_list" : "",
			"num_producers" : 20,
			"topic" : "my_feed"
		},
		"logging" : {
			"log_level" : "DEBUG"
			"log_file_location" : ""
		},
		"akka" : {
		    ... any overrides to the akka system
		}
	}
```
