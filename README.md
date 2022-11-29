## This git serves https://github.com/oracle/graal/issues/5522 and https://github.com/linghengqian/graalvm-trace-metadata-smoketest/issues/1

- Execute the following command to view the failure result.

```shell
sdk use java 22.3.r11-grl
gu install native-image
sudo apt-get install build-essential libz-dev zlib1g-dev -y
./gradlew -Pagent clean test
./gradlew metadataCopy --task test
./gradlew clean nativeTest
```