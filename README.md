# kie-wb-distributions

## Why do we need one more kie-wb-distribution?

We had an issue with uploading artifacts built in Java 17. The changes in this repository help to use custom process variables in Bussiness Central. Try it out!

## How to build Business Central?

1. Run the following command in the project's root path.
<br>`mvn clean install -e`

2. Once the building is completed, go to
<br>`business-central-parent -> jbpm-server-distribution -> target -> jbpm-server-7.74.0-SNAPSHOT-dist.zip`

3. Unzip the jbpm-server-7.74.0-SNAPSHOT-dist.zip and go to
<br>`standalone -> deployments -> business-central.war`

## Parent POMs and Inheritance

<a href="https://ibb.co/SJ5vFYz"><img src="https://i.ibb.co/d7jK8CR/pom.png" alt="pom" border="0"></a>

1. <b>jboss-parent.pom.xml:</b>

This POM acts as a top-level parent and defines common configurations and properties shared across various projects within the `org.jboss` group.
It serves as the foundation for maintaining a consistent set of settings throughout the organization.

2. <b>kie-parent.pom.xml:</b>

The `kie-parent.pom.xml` serves as an intermediate parent in our hierarchy.
It references the `jboss-parent.pom.xml` as its parent, effectively inheriting the common configurations and properties defined at the top level.
The purpose of this POM is to further refine configurations specific to our projects under the `org.kie` group.

3. <b>pom.xml (Project-Specific POM):</b>

The project-specific POM (`pom.xml`) is the main POM for an individual project.
It references the `kie-parent.pom.xml` as its parent, inheriting configurations from both `kie-parent.pom.xml` and indirectly from `jboss-parent.pom.xml`.
This setup ensures that our project adheres to the organization-wide standards while still allowing project-specific customizations.

## Versions and differences

### JBoss parent
1. JBoss parent version: `40-SNAPSHOT`
2. `maven-jar-plugin` version: from `3.3.0` to `3.1.0`
3. `maven.compiler.target` version: from `11` to `1.8`
4. `maven.compiler.source` version: from `11` to `1.8`
5. `requireMavenVersion` version: from `3.6.2` to `3.2.5`
6. from `<systemPropertyVariables/>` to `<systemProperties>`
7. removed: `versions-maven-plugin`

### Kie parent
1. Kie parent version: `7.74.0-SNAPSHOT`
2. `logback-core` version: from `1.4.7` to `1.2.9`
3. `commons-cli` version: from `1.5.0` to `1.4`
4. `commons-configuration` version: from `1.10` to `1.6`
5. `commons-digester` version: from `2.1` to `1.8`
6. `commons-fileupload` version: from `1.5` to `1.4`
