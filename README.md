# LicenseCollector
Illustrates the failure of the license-gradle-plugin under when coupled with Gradle 3.3 and Android Gradle plugin 2.3.0

* Working scenario
  * Android Gradle Plugin at version 2.0.0 in build.gradle
  * Gradle at version 2.10 in gradle/wrapper/gradle-wrapper.properties
  
* Failing scenario  
  * Android Gradle Plugin at version 2.3.0 in build.gradle
  * Gradle at version 3.3 in gradle/wrapper/gradle-wrapper.properties

Error reported with the newer versions:
> FAILURE: Build failed with an exception.
> 
> \* What went wrong:
> Execution failed for task ':downloadLicenses'.
> \> Could not get unknown property 'source' for object of type org.gradle.api.internal.artifacts.dependencies.DefaultSelfResolvingDependency.
> 
> \* Try:
> Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output.
