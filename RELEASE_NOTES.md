### Version 2.2 (April 12, 2015)

* Usage of [docker-java library](https://github.com/docker-java/docker-java) version 1.1.0.

### Version 2.1 (March 24, 2015)

* Renamed property `registry` to `registryCredentials` for plugin extension and tasks implementing `RegistryCredentialsAware` to better indicate its purpose.
_Note:_ This is a breaking change.

### Version 2.0.3 (March 20, 2015)

* Allow for specifying port bindings for container start command. - [Issue 30](https://github.com/bmuschko/gradle-docker-plugin/issues/30).
* Throw an exception if an error response is encountered - [Issue 37](https://github.com/bmuschko/gradle-docker-plugin/issues/37).
* Upgrade to Gradle 2.3.

### Version 2.0.2 (February 19, 2015)

* Set source and target compatibility to Java 6 - [Issue 32](https://github.com/bmuschko/gradle-docker-plugin/issues/32).

### Version 2.0.1 (February 10, 2015)

* Extension configuration method for `DockerJavaApplicationPlugin` needs to be registered via extension instance - [Issue 28](https://github.com/bmuschko/gradle-docker-plugin/issues/28).

### Version 2.0 (February 4, 2015)

* Upgrade to Gradle 2.2.1 including all compatible plugins and libraries.

### Version 0.8.3 (February 4, 2015)

* Add project group to default tag built by Docker Java application plugin - [Issue 25](https://github.com/bmuschko/gradle-docker-plugin/issues/25).

### Version 0.8.2 (January 30, 2015)

* Expose method for task `Dockerfile` for providing vanilla Docker instructions.

### Version 0.8.1 (January 24, 2015)

* Usage of [docker-java library](https://github.com/docker-java/docker-java) version 0.10.5.
* Correctly create model instances for create container task - [Issue 19](https://github.com/bmuschko/gradle-docker-plugin/issues/19).

### Version 0.8 (January 7, 2014)

* Allow for pushing to Docker Hub - [Issue 18](https://github.com/bmuschko/gradle-docker-plugin/issues/18).
* Better handling of API responses.
* Note: Change to plugin extension. The property `docker.serverUrl` is now called `docker.url`. Instead of `docker.credentials`, you will need to use `docker.registry`.

### Version 0.7.2 (December 23, 2014)

* `Dockerfile` task is always marked UP-TO-DATE after first execution - [Issue 13](https://github.com/bmuschko/gradle-docker-plugin/issues/13).
* Improvements to `Dockerfile` task - [Pull request 16](https://github.com/bmuschko/gradle-docker-plugin/pull/16).
    * Fixed wrong assignment of key field in  environment variable instruction.
    * Allow for providing multiple ports to the expose instruction.

### Version 0.7.1 (December 16, 2014)

* Fixed entry point definition of Dockerfile set by Java application plugin.

### Version 0.7 (December 14, 2014)

* Allow for properly add user-based instructions to Dockfile task with predefined instructions without messing up the order. - [Issue 12](https://github.com/bmuschko/gradle-docker-plugin/issues/12).
* Renamed task `dockerCopyDistTar` to `dockerCopyDistResources` to better express intent.

### Version 0.6.1 (December 11, 2014)

* Allow for setting path to certificates for communicating with Docker over SSL - [Issue 10](https://github.com/bmuschko/gradle-docker-plugin/issues/10).

### Version 0.6 (December 7, 2014)

* Usage of [docker-java library](https://github.com/docker-java/docker-java) version 0.10.4.
* Added Docker Java application plugin.
* Better documentation.

### Version 0.5 (December 6, 2014)

* Fixed implementations of tasks `DockerPushImage` and `DockerCommitImage` - [Issue 11](https://github.com/bmuschko/gradle-docker-plugin/issues/11).

### Version 0.4 (November 27, 2014)

* Added task for creating a Dockerfile.

### Version 0.3 (November 23, 2014)

* Usage of [docker-java library](https://github.com/docker-java/docker-java) version 0.10.3.
* Changed package name to `com.bmuschko.gradle.docker`.
* Changed group ID to `com.bmuschko`.
* Adapted plugin IDs to be compatible with Gradle's plugin portal.

### Version 0.2 (June 19, 2014)

* Usage of [docker-java library](https://github.com/docker-java/docker-java) version 0.8.2.
* Provide custom task type for push operation.
* Support for using remote URLs when building image - [Issue 3](https://github.com/bmuschko/gradle-docker-plugin/issues/3).

### Version 0.1 (May 11, 2014)

* Initial release.