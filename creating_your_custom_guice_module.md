# Creating Your Custom Guice Module

Guice can be used in Orienteer as an ["Injection engine"](https://en.wikipedia.org/wiki/Dependency_injection). 

[Here](http://blog.mathieu.carbou.me/post/60455011429/automatically-discover-guice-modules-and-override) you can check how to add your own guiece module. In short:

1. Implement your own Guice module.
2. If it should override some existing configurations, mark it by annotation @OverrideModule.
3. Add record for your class to META-INF/services/com.google.inject.Module


