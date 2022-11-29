## This git serves https://github.com/linghengqian/graalvm-trace-metadata-smoketest/issues/1
- Execute the following command to view the failure result.
```shell
./gradlew -Pagent clean test
./gradlew metadataCopy --task test
./gradlew clean nativeTest
```