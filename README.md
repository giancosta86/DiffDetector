# DiffDetector

*Simple RESTful architecture for binary comparison*


## Introduction


**DiffDetector** is a small architecture dedicated to showing how to employ Spring MVC with other technologies - such as JavaFX - via a dedicated SDK layer that encapsulates calls to the web services.


![Architecture](https://github.com/giancosta86/DiffDetector/blob/master/architecture.png "Architecture")


DiffDetector consists of 4 components:

* [DiffDetector-core](https://github.com/giancosta86/DiffDetector-core) - containing the core model elements

* [DiffDetector-web](https://github.com/giancosta86/DiffDetector-web) - that implements and runs web services via Spring MVC

* [DiffDetector-sdk](https://github.com/giancosta86/DiffDetector-sdk) - a Java library for transparently interacting with the web services

* [DiffDetector-fx](https://github.com/giancosta86/DiffDetector-fx) - a simple JavaFX app that employs the SDK for web calls


All the projects depend on well-known open source libraries; the build process is managed by Gradle, via a few additional plugins:

* [Aurora](https://github.com/giancosta86/Aurora) - to have a common, elegant build pipeline

* [MoonLicense-Gradle](https://github.com/giancosta86/MoonLicense-Gradle) - to add a copyright header to files

* [MoonDeploy-Gradle](https://github.com/giancosta86/MoonDeploy-Gradle) - to automatically create deployment descriptors for [MoonDeploy](http://gianlucacosta.info/moondeploy)