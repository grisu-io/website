---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

Grisu.io is a tiny framework that will help you build your Java microservices more quickly and efficiently.

The codebase is organised in multiple modules in order to clearly serve different purposes:

- [core library](https://github.com/grisu-io/core) / This is the main library of the whole framework and it is referenced by other packages from the _Grisu family_. It provides common basic functionalities, such as a [MapBuilder.java](https://github.com/grisu-io/core/blob/master/src/main/java/io/grisu/core/utils/MapBuilder.java) or [MapUtils.java](https://github.com/grisu-io/core/blob/master/src/main/java/io/grisu/core/utils/MapUtils.java), a collection of common operators on maps or [GrisuException.java](https://github.com/grisu-io/core/blob/master/src/main/java/io/grisu/core/exceptions/GrisuException.java), a useful Exception class

- [pojo](https://github.com/grisu-io/pojo) / This library helps you create different and specialised Java classes whose properties must be automatically copied to/from other classes (eg. representational classes <--> dto <--> beans) within the same JVM or even wire-transfered. In fact the _pojo_ library provides a very easy and out-of-the-box mechanism to translate a pojo class into a JSON serialized string and viceversa.

- [usvcs](https://github.com/grisu-io/usvcs) / Here you have the annotations library used to map the microservices/nanoservices within your implementations. Thanks to this abstraction and actual implementations (eg. _usvcs-rabbitmq_) you can switch between a "monolithic" or "distributed" approach within minutes

- [usvcs-rabbitmq](https://github.com/grisu-io/usvcs-rabbitmq) / RabbitMQ implementation of the _usvcs_ package 

- [persistentpojo](https://github.com/grisu-io/persistentpojo) / This package defines (and provides tools for) pojos that must be persisted  

- [storage]() / Still to release as opensource project / Cassandra + Elastic Search implementation of the _persistentpojo_ interfaces

- [ee-core](https://github.com/grisu-io/ee-core) / convenience package to collect _java-ee_ utils
