The plugin is published to Sonatype, using [sbt-sonatype](https://github.com/xerial/sbt-sonatype).

## Publishing

See the [ossrh guide](http://central.sonatype.org/pages/ossrh-guide.html) to create an account with sonatype. Once you have an account you will need to [request access](https://issues.sonatype.org/browse/OSSRH-21756) to **com.gilt**. Finally, generate a pgp key and set up your [sonatype credentials](http://www.scala-sbt.org/release/docs/Using-Sonatype.html).

## Tag a New Version and Release

    sbt release

## Publishing to Sonatype

    sbt publishSigned

## Releasing a new version (not needed for -SNAPSHOT versions)

After publishing as above:

    sbt sonatypeRelease