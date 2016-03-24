# Creating Your Custom Guice Module
It can be done according the following approach: http://blog.mathieu.carbou.me/post/60455011429/automatically-discover-guice-modules-and-override

1. Implement your own Guice Module
2. If it should override some existomg configuration mark it by annotation @OverrideModule
3. Add record for your class to META-INF/services/com.google.inject.Module


