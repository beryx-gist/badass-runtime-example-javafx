[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/beryx-gist/badass-runtime-example-javafx/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/beryx-gist/badass-runtime-example-javafx/master.svg?label=Build)](https://travis-ci.org/beryx-gist/badass-runtime-example-javafx)

## Badass Runtime Plugin Example: JavaFX Application ##

A small JavaFX 11 non-modular application that shows how to use the [Badass Runtime Plugin](https://github.com/beryx/badass-runtime-plugin/).

It allows you create custom runtime image of your application and a platform-specific installer for it.

### Usage
**Running with gradle:**
```
./gradlew run
```

A window containing the text `Hello, OpenJFX!` should appear on the screen.


**Creating and executing a custom runtime image:**
```
./gradlew runtime
cd build/image/bin
./hellofx
```

A window containing the text `Hello, OpenJFX!` should appear on the screen.


**Creating a platform-specific installer:**
```
./gradlew jpackage
```

The above command will generate the platform-specific installers in the `build/jpackage` directory.
