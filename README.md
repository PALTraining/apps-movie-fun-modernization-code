In this lab, you will learn about database migrations in a distributed system. Database definition files are intentionally maintained outside of the deployable application or service and migrations are executed with Gradle. This gives more control over when migrations happen, which is necessary for complex deployments.

# Movie Fun!

Smoke Tests require server running on port 8080 by default.

## Build JAR ignoring tests

```bash
$ ./gradlew clean build -xtest
```

## Run Smoke Tests against specific URL

```bash
$ MOVIE_FUN_URL=http://moviefun.example.com ./gradlew test
```
