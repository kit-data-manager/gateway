# Gateway

This is the simplest Spring Cloud Gateway implementation possible. The idea is to configure all routes via a `application.yml` instead of coding the routes into the gateway. See `config_example` for an example and some documentation links for the configuration.

- [About the difference to a reverse proxy](https://www.baeldung.com/cs/api-gateway-vs-reverse-proxy), see especially [this section for a short Overview](https://www.baeldung.com/cs/api-gateway-vs-reverse-proxy#differences).


## Usage

If you want to run it straight from the repository (e.g., for development or compiling on the server):

```bash
# build only
./gradlew build
# run with config (also builds if this did not happen before)
./gradlew run --args="--spring.config.location=config_example/application.yml"
```

If you only use the JAR file on your server:

```bash
java -jar gateway.jar --spring.config.location=path/to/config/file.yml
```

> **Note**
> 
> Remember to restart the application if you change the configuration file.
