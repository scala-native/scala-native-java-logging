# scala-native-java-logging

[![CI](https://github.com/scala-native/scala-native-java-logging/actions/workflows/ci.yml/badge.svg)](https://github.com/scala-native/scala-native-java-logging/actions/workflows/ci.yml)

`scala-native-java-logging` is a BSD-licensed reimplementation of the `java.logging` API for Scala Native.
It enables this API in Scala Native projects.

Ported from https://github.com/scala-js/scala-js-java-logging.

## Usage

Simply add the following line to your sbt settings:

```scala
libraryDependencies += "org.scala-native" %%% "scala-native-java-logging" % "1.0.0"
```

If you have a `crossProject`, the setting must be used only in the JS part:

```scala
lazy val myCross = crossProject.
  ...
  nativeSettings.(
    libraryDependencies += "org.scala-native" %%% "scala-native-java-logging" % "1.0.0"
  )
```

## Work in Progress / linking errors

This library is a work in progress.
There are still many classes and methods that have not been implemented yet.
If you use any of those, you will get linking errors.

Feel free to [contribute](./CONTRIBUTING.md) to extend the set of supported
classes and methods!

## License

`scala-native-java-logging` is distributed under the
[BSD 3-Clause license](./LICENSE.txt).

## Contributing

Follow the [contributing guide](./CONTRIBUTING.md).
