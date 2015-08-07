# Test Utility for UAAS

This program tests UAAS web service.


## Requirements

Test Utility requires the following software:

- Linux/Unix/Windows
- Java 7 or higher
- Maven 3.2.1 or higher


## Assemble program
In the command line
```
mvn clean package
```

## Run program
Example
```
java -jar TestUtility.jar "pathToConfigFile"
```

## Config file

[examples/properties.config](examples/properties.config)

## Input file example

[examples/testc.csv](examples/testc.csv)

## Convertion algorithms

[docs](docs)

## Testing
For start test service launch com.ts.endpoint.WSPublisher in ws folder
For using test service change host in properties file and replace string
SOAPManagerStat smi = new HTTPManagerStatImpl(PropConfig.host, new HTTPParseResponseImpl(), new HTTPRequestCreatorImpl());
with
SOAPManagerStat smi = new HTTPManagerStatImpl(PropConfig.host, new HTTPParseResponseTestImpl(), new HTTPRequestCreatorTestImpl());
in com.ts.App class in TextUtility folder.
