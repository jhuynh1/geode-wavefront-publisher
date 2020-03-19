## geode-wavefront-publisher

### How to Build
./gradlew shadowJar

### How to Deploy
Here is an example command to start a locator

start locator --name=locator --classpath=/Users/jhuynh/geode-wavefront-publisher/build/libs/geode-wavefront-publisher-1.0-SNAPSHOT-all.jar --J=-Dgeode-wavefront-api-token=someapitoken --J=-Dgeode-wavefront-prefix=wavefront.jhuynh --J=-Dgeode-wavefront-source=apache.geode


### Configuration Parameters


TODO
