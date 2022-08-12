# Gateway

This is the simplest Spring Cloud Gateway implementation possible. The idea is to configure all routes via a `application.yml` instead of coding the routes into the gateway. See `config_example` for an example and some documentation links for the configuration.

- [About the difference to a reverse proxy](https://www.baeldung.com/cs/api-gateway-vs-reverse-proxy), see especially [this section for a short Overview](https://www.baeldung.com/cs/api-gateway-vs-reverse-proxy#differences).


## Usage

```bash
# build
./gradlew build
# configure and run
cd build/libs
cp ../../config_example ./
java -jar gateway-0.0.1-SNAPSHOT.jar
```

Remember to restart the application if you change the configuration file.
