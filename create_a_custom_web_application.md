# Create a Custom Web Application


It's highly recommended to use Orienteer maven archetype to create your custom web application.

#### From latest snapshot

```bash
mvn archetype:generate \
  -DarchetypeGroupId=org.orienteer \
  -DarchetypeArtifactId=orienteer-archetype-war \
  -DarchetypeVersion=1.2-SNAPSHOT \
  -DarchetypeRepository=https://oss.sonatype.org/content/repositories/snapshots
```

#### From latest release

```bash
mvn archetype:generate \
  -DarchetypeGroupId=org.orienteer \
  -DarchetypeArtifactId=orienteer-archetype-war \
  -DarchetypeVersion=1.1
```
