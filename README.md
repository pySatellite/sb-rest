# HELLO SB REST

### build
```
$ ./gradlew clean

BUILD SUCCESSFUL in 605ms
1 actionable task: 1 executed
$ ls -l build
ls: cannot access 'build': No such file or directory
$ ./gradle test
zsh: permission denied: ./gradle
$ ./gradlew test

> Task :test
OpenJDK 64-Bit Server VM warning: Sharing is only supported for boot loader classes because bootstrap classpath has been appended

BUILD SUCCESSFUL in 4s
3 actionable tasks: 3 executed
$ ./gradlew jar

BUILD SUCCESSFUL in 759ms
2 actionable tasks: 1 executed, 1 up-to-date
$ ls -l build/libs
total 4
-rw-r--r-- 1 nori nori 2862 Feb 27 11:01 rest-service-0.0.1-SNAPSHOT-plain.jar
$ ./gradlew bootJar

BUILD SUCCESSFUL in 934ms
3 actionable tasks: 2 executed, 1 up-to-date

$ java -jar build/libs/rest-service-0.0.1-SNAPSHOT.jar
```