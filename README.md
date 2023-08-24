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

<a href="https://ibb.co/yqKVH2P"><img src="https://i.ibb.co/4pCJhkt/kie-wb-distributions.png" alt="kie-wb-distributions" border="0"></a>

## Versions and differences

### JBoss parent
1. JBoss parent version: from `36` to `40-SNAPSHOT`
2. `version.antrun.plugin` version: from `1.8` to `3.1.0`
3. `version.archetype.plugin` version: from `3.1.0` to `3.2.1`
4. `version.buildhelper.plugin` version: from `3.0.0` to `3.4.0`
5. `version.buildnumber.plugin` version: from `1.4` to `3.1.0`
6. `version.bundle.plugin` version: from `3.5.0` to `5.1.9`
7. `version.checkstyle.plugin` version: from `3.0.0` to `3.2.2`
8. `version.clean.plugin` version: from `3.1.0` to `3.2.0`
9. `version.compiler.plugin` version: from `3.8.0-jboss-2` to `3.11.0`
10. `version.dependency.plugin` version: from `3.1.1` to `3.5.0`
11. `version.deploy.plugin` version: from `2.8.2` to `3.1.1`
12. `version.download.plugin` version: from `1.4.1` to `1.7.0`
13. `version.ear.plugin` version: from `3.0.1` to `3.3.0`
14. `version.ejb.plugin` version: from `3.0.1` to `3.2.1`
15. `version.exec.plugin` version: from `1.6.0` to `3.1.0`
16. `version.enforcer.plugin` version: from `3.0.0-M2` to `3.3.0`
17. `version.gpg.plugin` version: from `1.6` to `3.1.0`
18. `version.help.plugin` version: from `3.1.0` to `3.4.0`
19. `version.injection.plugin` version: from `1.0.2` to `1.3`
20. `version.install.plugin` version: from `2.5.2` to `3.1.1`
21. `version.javadoc.plugin` version: from `3.0.1` to `3.5.0`
22. `version.jxr.plugin` version: from `2.5` to `3.3.0`
23. `version.license.plugin` version: from `1.16` to `2.0.1`
24. `version.plugin.plugin` version: from `3.5.2` to `3.9.0`
25. `version.pmd.plugin` version: from `3.10.0` to `3.21.0`
26. `version.rar.plugin` version: from `2.4` to `3.0.0`
27. `version.release.plugin` version: from `2.5.3` to `3.0.0`
28. `version.resources.plugin` version: from `3.1.0` to `3.3.1`
29. `version.shade.plugin` version: from `3.1.1` to `3.4.1`
30. `version.site.plugin` version: from `3.7.1` to `4.0.0-M8`
31. `version.sonar.plugin` version: from `3.6.0.1398` to `3.9.1.2184`
32. `version.source.plugin` version: from `3.0.1` to `3.3.0`
33. `version.surefire.plugin` version: from `2.22.0` to `3.1.0`
34. `version.war.plugin` version: from `3.2.2` to `3.3.2`
35. `version.zanata.plugin` version: from `4.4.3` to `4.6.2`
36. `version.plexus.archiver` version: from `3.6.0` to `4.7.1`
37. `version.checkstyle` version: from `8.19` to `8.34`
38. 

### Kie parent
1. Kie parent version: `7.74.0-SNAPSHOT`
2. `version.commons-fileupload` version: from `1.5` to `1.4`
3. `version.org.reflections` version: from `0.9.11` to `0.10.2`
4. `version.xalan` version: from `2.7.3` to `2.7.2`
5. `version.org.apache.cxf` version: from `3.5.5` to `3.4.0`
6. `version.net.byte-buddy` version: from `1.10.3` to `1.14.4`
