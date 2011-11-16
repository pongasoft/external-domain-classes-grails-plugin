Introduction
============
The goal of this plugin is to be able to declare a domain class outside the environment of a grails application and yet still be considered a domain class by grails

How to use
==========

In order to use the plugin:

* install the plugin
* _mark_ your domain classes by annotating them with the `grails.persistence.Entity` annotation (which unfortunately adds a ton of grails and spring dependencies to your code :()
* define a `grails.external.domain.packages` property in your config file (`Config.groovy`). Example:
      
        grails.external.domain.packages = ['com.acme.domain1', 'com.acme.domain2']

How to package the plugin
=========================

Simply run:

    grails package-plugin