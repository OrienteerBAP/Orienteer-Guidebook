# Create REST API

First of all, try to consider to use [OOB REST functionality](resthttp_api.md). It's pretty wide to cover different business needs: especially through server-side scripting (OFunction).
But if you need to have your own REST API in any case: to add it is extremly easy.

Add the following snippets into `pom.xml` of your project.

**To root `project` xml element:**
```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>org.glassfish.jersey</groupId>
            <artifactId>jersey-bom</artifactId>
            <version>2.23.1</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```

**To a list of projects:**
```xml
<dependency>
    <groupId>org.glassfish.jersey.containers</groupId>
    <artifactId>jersey-container-servlet</artifactId>
</dependency>

<dependency>
    <groupId>org.glassfish.jersey.test-framework.providers</groupId>
    <artifactId>jersey-test-framework-provider-bundle</artifactId>
    <type>pom</type>
    <scope>test</scope>
</dependency>
```
Also make sure that you use Servlet 3.0+ compatible web container.