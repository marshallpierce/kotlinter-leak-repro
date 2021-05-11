A reproduction of https://github.com/jeremymailen/kotlinter-gradle/issues/204.

Open up VisualVM, or use jcmd's GC.class_histogram, or your preferred mem leak monitoring tool, and then format kotlin repeatedly.

```
./gradlew --stop
repeat 100 ./gradlew formatKotlin
```
