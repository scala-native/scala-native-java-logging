# Contributing guidelines

See the [contributing guidelines of Scala Native core](https://github.com/scala-native/scala-native/blob/main/CONTRIBUTING.md).
The same guidelines apply to this repository.

## Very important notice

`scala-native-java-logging` contains a reimplementation of part of the JDK in Scala Native itself.

***To contribute to this code, it is strictly forbidden to even look at the
source code of the Oracle JDK or OpenJDK!***

This is for license considerations: these JDKs are under a GPL-based license,
which is not compatible with our BSD 3-clause license.

The only existing JDK source code that we can look at is the dead Apache
Harmony project.
