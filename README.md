# docker-logstash-filebeat-sandbox
Logstash + Filebeat sandbox to test Elastic configurations

## Description
It can be difficult to pinpoint filebeat and logstash configuration problems, alter configurations in a quick manner, and test them timely and efficiently. This attempts to help with this.

This project will use a filebeat and logstash image to send a log file to a logstash instance and output the result to stdout.

## Prerequisites
- Maven

## Up and running
1. Create a log file under volumes/logs/
2. Create a logstash configuration to test under volumes/logstash-test.conf
3. Run: "sudo chown root:root volumes/filebeat/filebeat.yml"
3. mvn docker:run
