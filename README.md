scala
=====

This is a Grails Plugin that enable the usage of Scala code in Grails Web projects.


Distribution
============

grails-scala-<version>.zip for the plugin source distribution
  -- this is the recommended version, because the binary version of this plugin doesn't contain required jars


Dependencies
============

* a Servlet container to run the Web application, as required by the used version of Grails
* Scala (as specified in plugin descriptor) and related dependencies


Installation
============

In BuildConfig.groovy of the webapp, under the plugins section (at the end of the file) add:

    compile ":scala:<version>"

then run grails refresh-dependencies, grails clean , then grails compile , and the plugin should be installed.
In case of Errors during plugin installation, Set log level to 'warn' in BuildConfig.groovy to get more information, and retry.
Instead of the compile it's possible even to use runtime, and in that case simply running a grails console should be enough.


Documentation
=============

See the Plugin documentation (sources under src/docs/), or the "live" version here:
[grails-scala docs](http://smartiniongithub.github.com/grails-scala/)

Home Page for the project (and sources) on GitHUB:
[grails-scala](https://github.com/smartiniOnGitHub/grails-scala/)

Note that this plugin uses the utility jar groovytransforms, since 0.3 hosted at JCenter (BinTray):
[groovytransforms](http://dl.bintray.com/smartiniontray/releases/)
and that repository has been added manually in Plugin configuration (because the Plugin uses a legacy Grails release).


License
=======

Licensed under the terms of the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
