# p6spy-it-spring-boot
p6spy integration with spring boot, for necessary spring-boot related config changes, see files:
* `application.yml` - modified: `spring.datasource.url` holding `p6spy`
* `build.gradle` - holding  `dependency { compile "p6spy:p6spy:3.0.0"`
* as well as optional `spy.properties` holding the p6spy specific options

To give it a test try, run:

    rm -rf spy.log; ./gradlew clean test; tail spy.log
