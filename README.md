This is for the development of the dashboards maybe alerts in Splunk for CBTC project. 
Currently, it only draws data from iams-prod, Kafka clusters, via Splunk connector for Kafka. 
There is a Splunk connect process running in csedev-yshen with Splunk connector registered. 
The Splunk connector hosted by the Kafka connect process relays the iams-prod Kafka messages to the HEC (HTTP Endpoint Collector) of Splunk
at a Splunk instance running in a podman image in csedev-yshen. Then the HEC put the received messages in index cbtc_messages in sourcetype _json. 

With query
index=cbtc_messages 

it is possible to query the message received. Then the messages are formated by the dashboard in this project. 
