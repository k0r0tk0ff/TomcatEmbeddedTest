Project for launch Tomcat Embedded from jar archive

Use maven plugins for pack to one archive 
1) Tomcat Embedded
2) Simple jsp page

Add resources files (jsp files) to jar -

<resources>
    <resource>
        <directory>src/main/webapp</directory>
            <targetPath>META-INF/resources</targetPath>
    </resource>
</resources>


Create jar archive:
mvn package

run:
java -jar TomcatEmbeddedTest-1.0-SNAPSHOT-jar-with-dependencies.jar