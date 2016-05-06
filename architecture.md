# Architecture

Image: architecture


## Modules

| Module | Description |
| -- | -- |
| Orienteer Core | The core module of Orienteer, which contains its operation essentials |
| Orienteer Graph | The module that makes working with graphs easier and friendlier|
| Orienteer Pages | The basic CMS functionality |
| Orieneer PivotTable | Integration with [JS Pivot Table](http://nicolas.kruchten.com/pivottable/examples/)|
| Orienteer Standalone | The wrapper used to run Orienteer in the standalone mode|
| Orienteer WAR | The module that creates a **.war* file with default Orienteer modules for deploying Orienteer as a web application on an application server|
| Orienteer Maven Jar Archetype | The Maven Archetype toolkit to bootstrap your own module for Orienteer|
| Orienteer Maven War Archetype | The Maven Archetype toolkit to bootstrap your custom web application on top of Orienteer|


## Libraries

| Library| Role |
| -- | -- |
| [OrientDB](https://github.com/orientechnologies/orientdb) | A paradigmatic NoSQL database to provide the Persistence Layer in Orienteer|
| [Apache Wicket](http://wicket.apache.org/) | A lightweight and extremely powerful web framework |
| [wicket-orientdb](https://github.com/OrienteerDW/wicket-orientdb) | An utility library for comfort work with OrientDB in Apache Wicket |
| [Google Guice](https://github.com/google/guice) | A framework for dependencies injection | 

All dependencies can be found here: [![Dependency Status](https://www.versioneye.com/user/projects/572bd228a0ca350034be6f9d/badge.svg?style=flat)](https://www.versioneye.com/user/projects/572bd228a0ca350034be6f9d)
