# Gateway

This is the simplest Spring Cloud Gateway implementation possible. The idea is to configure all routes via a `application.yml` instead of coding the routes into the gateway. See `config_example` for an example and some documentation links for the configuration.

## Build

`./gradlew build`

## Start

```bash
cd build/libs
cp ../../config_example ./
java -jar gateway-0.0.1-SNAPSHOT.jar
```

Remember to restart the application if you change the configuration file.
