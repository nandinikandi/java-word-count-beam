# Nandini Kandi

## Use Maven archetype to fetch a project.
`mvn archetype:generate  -D archetypeGroupId=org.apache.beam -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples -D archetypeVersion=2.36.0  -D groupId=org.example -D artifactId=word-count-beam  -D version="0.1"  -D package=org.apache.beam.examples  -D interactiveMode=false`

## Create a input.txt file
 Add Shakesphere sonnets content into input.txt

## Run a pipeline

Use the command in git bash
`$ mvn compile exec:java -Dexec.mainClass=org.apache.beam.examples.WordCount -Dexec.args="--inputFile=input.txt --output=counts" -Pdirect-runner`

