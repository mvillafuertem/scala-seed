:warning: PLEASE, DO NOT EDIT THIS FILE.
IT IS AUTOGENERATE YOU SHOULD EDIT `modules/docs/src/main/mdoc/README.md`
WITH THE COMMAND `sbt docs/mdoc`

---


# @PROJECT_NAME@

[![Donate](https://img.shields.io/badge/donate-PayPal-green.svg?logo=paypal)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=HE7K7HLJJBVWN&currency_code=EUR&source=url)
[![Scala](https://img.shields.io/badge/scala-@SCALA_VERSION@-red.svg?logo=scala&logoColor=red)](https://github.com/scala/scala/releases)
[![Java](https://img.shields.io/badge/jdk-@JAVA_VERSION@-orange.svg?logo=java&logoColor=white)](https://www.oracle.com/technetwork/java/javase/11all-relnotes-5013287.html)
[![Sbt](https://img.shields.io/badge/sbt-@SBT_VERSION@-blue.svg?logo=sbt)](https://github.com/sbt/sbt/releases)
[![Scala CI](https://github.com/mvillafuertem/scala-seed/workflows/scalaci/badge.svg)](https://github.com/mvillafuertem/scala-seed/actions?query=workflow%3A%22scalaci%22)

****

@PROJECT_NAME@ is a project ...

****


## [UI](https://mvillafuertem.github.io/scala-seed)

### Development

```shell

sbt "project ui;~fastOptJS"

yarn --cwd modules/ui/ webpack serve --env BUILD_KIND=development --mode=development --config webpack/scala.webpack.config.js

```

### Production

```shell

sbt "project ui;fullOptJS"

yarn --cwd modules/ui/ webpack-cli --env BUILD_KIND=production --mode=production --config webpack/scala.webpack.config.js

```