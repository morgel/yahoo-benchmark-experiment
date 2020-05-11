# yahoo-benchmark-experiment

To build the generator:
---
lein uberjar

To setup the generator on redis (ensure values in properties file are correct):
---
java -jar setup/target/uberjar/setup-0.1.0-SNAPSHOT-standalone.jar -n

To execute the generator in the background:
---
nohup java -jar target/uberjar/setup-0.1.0-SNAPSHOT-standalone.jar -r -t 17000 > /dev/null 2>&1 &
