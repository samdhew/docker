FROM amazoncorretto:17-alpine

# Install curl and download NewRelic APM for Java
RUN apk --no-cache add curl
curl -O https://download.newrelic.com/newrelic/java-agent/newrelic-agent/current/newrelic-java.zip
unzip newrelic-java.zip
