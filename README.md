spring-data-elasticsearch-mvn-config
====================================

Problem:
Missing plugin com.springsource.bundlor:com.springsource.bundlor.maven:1.0.0.RELEASE

Solution 1:
Add this to the pom.xml (not prefered). 

    <pluginRepositories>
        <pluginRepository>
            <id>com.springsource.repository.bundles.release</id>
            <url>http://repository.springsource.com/maven/bundles/release</url>
        </pluginRepository>
    </pluginRepositories>

Solution 2:

Create a file 'settings.xml' in your .m2 folder and add this fragment to it.

    <pluginRepository>
        <id>com.springsource.repository.bundles.release</id>
        <url>http://repository.springsource.com/maven/bundles/release</url>
    </pluginRepository>
    
I have added entire settings.xml as an example.    
        


