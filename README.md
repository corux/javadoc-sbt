# javadoc sbt

Generate java api docs with javadoc.

## Installation

In your own project, create or edit `project/plugins.sbt` and add

    addSbtPlugin("de.corux" % "javadoc-sbt" % "0.1.0-SNAPSHOT")
    resolvers += "corux-releases" at "http://tomcat.corux.de/nexus/content/repositories/releases/"
    resolvers += "corux-snapshots" at "http://tomcat.corux.de/nexus/content/repositories/snapshots/"

In your `build.sbt` add

    seq(javadoc.JavadocPlugin.javadocSettings: _*)

## Usage

Use the new `javadoc` task to generate api documentation for your java
source code (as opposed to scala code, for which you can use the normal
`doc` task).

All original work goes to Bart Schuller.
