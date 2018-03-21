# bazel-build-spring-boot

This is a very basic bazel config to build Spring Boot using a rule from salesforce's team.

To install Bazel see https://docs.bazel.build/versions/master/getting-started.html

Build command:
```sh
$ bazel build //:spring-boot-sample-jetty
```

To run the generated jar:
```sh
$ java -jar bazel-genfiles/spring-boot-sample-jetty_springboot.jar
```
