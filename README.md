# Pivotal Cloud Foundry - Spin and Scale your app in Cloud in Few minutes 

### Pre-Requisites if building the Jar in Local

Below tools needs to be installed in your machine,
- Java
- Maven

### Receipe

- Create a PCF account - https://account.run.pivotal.io/z/uaa/sign-up - You get a free tier for a year ( I guess ) just like AWS.
- Install the CLI tool for PCF - https://docs.run.pivotal.io/cf-cli/install-go-cli.html
- Build your jar locally (this example) or from a artifactory location
- Run the `cf push` command to deploy your application

### Useful Links

- https://docs.cloudfoundry.org/devguide/deploy-apps/manifest.html#memory - Manifest commands
- http://spring.io/guides/gs/rest-service/ - Build a Restful Service
- https://github.com/spring-guides/gs-rest-service/tree/master/complete - Sample Service to Deploy

### Useful Commands

```
cf login -a api.run.pivotal.io

cf login [-a API_URL] [-u USERNAME] [-p PASSWORD] [-o ORG] [-s SPACE]

cf push <YOUR-APP-NAME> -p <YOUR-JAR-LOCATION> https://github.com/cloudfoundry/java-buildpack.git -m 1G
```
