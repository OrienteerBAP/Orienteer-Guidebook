# Testing Your Solution

You can use Orienteer testing micro-framework to test a module you develop for Orienteer or an application you build within Orienteer framework.

Is this about using orienteer as a framework or about testing a module for orienteer?


Actually both: and for custom module or custom web application on top of Orienteer. Whenever Orienteer is being used: this info might be useful


There are 2 ways to enable Orienteer testing framework:

##Use of OrienteerTestRunner

    @RunWith(OrienteerTestRunner.class)
    @Singleton
    public class TestMyFunctionality
    {
       @Inject
       private OrienteerTester tester;
       
       ....
    }

##Use of OrienteerRule

    public class TestMyFunctionality
    {
       @Rule
       public OrienteerRule orienteer = new OrienteerRule();

       @Inject
       private OrienteerTester tester;

       ....
    }
##Configuring custom Orienteer based project

A long with common dependency on Orienteer

    <dependency>
        <groupId>org.orienteer</groupId>
        <artifactId>orienteer-core</artifactId>
        <version>${orienteer.version}</version>
    </dependency>

include dependency to Orienteer and wicket-orientdb tests

    <dependency>
        <groupId>org.orienteer</groupId>
        <artifactId>orienteer-core</artifactId>
        <version>${orienteer.version}</version>
        <type>test-jar</type>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>ru.ydn.wicket.wicket-orientdb</groupId>
        <artifactId>wicket-orientdb</artifactId>
            <version>${wicket.orientdb.version}</version>
        <type>test-jar</type>
        <scope>test</scope>
    </dependency>
And that's all. You are ready to...
