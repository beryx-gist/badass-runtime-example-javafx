[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/beryx-gist/badass-runtime-example-javafx/blob/master/LICENSE)
[![Build Status](https://github.com/beryx-gist/badass-runtime-example-javafx/workflows/Gradle%20Build/badge.svg)](https://github.com/beryx-gist/badass-runtime-example-javafx/actions?query=workflow%3A%22Gradle+Build%22)


## Badass Runtime Plugin Example: JavaFX Application ##

A small JavaFX 11 non-modular application that shows how to use the [Badass Runtime Plugin](https://github.com/beryx/badass-runtime-plugin/).

It allows you to create custom runtime image of your application and a platform-specific installer for it.

### Usage
**Running with gradle:**
```
./gradlew run
```

The following window should appear on the screen:

<img src="https://github.com/beryx-gist/badass-runtime-example-javafx/raw/master/doc/app.png">


**Creating and executing a custom runtime image:**
```
./gradlew runtime
cd build/image/bin
./hellofx
```

A window containing the text `Hello JavaFX` should appear on the screen.


**Creating a platform-specific installer:**
```
./gradlew jpackage
```

The above command will generate the platform-specific installers in the `build/jpackage` directory.

:bulb: You can check the artifacts produced by the [GitHub actions used to build this project](https://github.com/beryx-gist/badass-runtime-example-javafx/actions?query=workflow%3A%22Gradle+Build%22) and download an application package for your platform (such as [from here](https://github.com/beryx-gist/badass-runtime-example-javafx/actions/runs/224938848)).
