## geode-wavefront-publisher
Pick either to download a prebuilt jar or build from source

### 1a. Download a prebuilt jar
[geode-wavefront-publisher.jar](https://bintray.com/jasonhuynh/jhuynh1-maven/download_file?file_path=com%2Fgithub%2Fjhuynh1%2Fgeode%2Fwavefront%2Fgeode-wavefront-publisher%2F1.0%2Fgeode-wavefront-publisher-1.0-all.jar)

### 1b. Build
#### Clone the repo
git clone https://github.com/jhuynh1/geode-wavefront-publisher.git

#### Build the jar
./gradlew shadowJar

### 2. Obtain Wavefront API token

### 3. Deploy
Here is an example command to start a locator and server

start locator --name=locator --classpath=/Users/jhuynh/geode-wavefront-publisher/build/libs/geode-wavefront-publisher-1.0-SNAPSHOT-all.jar --J=-Dgeode-wavefront-api-token=someapitoken --J=-Dgeode-wavefront-prefix=wavefront.jhuynh --J=-Dgeode-wavefront-source=apache.geode

start server --name=server --classpath=/Users/jhuynh/geode-wavefront-publisher/build/libs/geode-wavefront-publisher-1.0-SNAPSHOT-all.jar --J=-Dgeode-wavefront-api-token=someapitoken --J=-Dgeode-wavefront-prefix=wavefront.jhuynh --J=-Dgeode-wavefront-source=apache.geode


### Configuration Parameters
|name|description|default|
|-----|-----|-----|
|geode-wavefront-prefix| the wavefront prefix for metrics| wavefront |
|geode-wavefront-source| the source name for the metric| apache.geode|
|geode-wavefront-api-token| the wavefront api token| N/A|
