# Development Environment

List of all software development tools that I use.


## SonarQube

### Configuration

Add this following configuration to `settings.xml` file located on your host machine `~/.m2` folder.

```xml
<settings>
    <pluginGroups>
        <pluginGroup>org.sonarsource.scanner.maven</pluginGroup>
    </pluginGroups>
    <profiles>
        <profile>
            <id>sonar</id>
            <activation>
    <activeByDefault>true</activeByDefault>
            </activation>
        </profile>
     </profiles>
</settings>
```

If you stomp on the problem with SonarQube Docker image that Elastic search max virtual memory access is too low, go check the solution: <https://stackoverflow.com/questions/51445846/elastic-search-max-virtual-memory-areas-vm-max-map-count-65530-is-too-low-inc>
