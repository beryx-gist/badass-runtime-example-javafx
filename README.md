[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/beryx-gist/badass-runtime-example-javafx/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/beryx-gist/badass-runtime-example-javafx/master.svg?label=Build)](https://travis-ci.org/beryx-gist/badass-runtime-example-javafx)

## Badass Runtime Plugin Example: JavaFX Application ##

A small JavaFX 11 non-modular application that shows how to use the [Badass Runtime Plugin](https://github.com/beryx/badass-runtime-plugin/).

The plugin is configured in `build.gradle` as follows:

```
plugins {
    id 'application'
    id 'org.openjfx.javafxplugin' version '0.0.7'
    id 'org.beryx.runtime' version '1.1.5'
}


repositories {
    mavenCentral()
}

javafx {
    modules = ['javafx.controls']
}

application {
    mainClassName = "org.example.hellofx.Launcher"
    applicationName = 'hellofx'
}
```

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
