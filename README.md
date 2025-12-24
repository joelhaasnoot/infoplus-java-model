infoplus-model-java
=====

Library containing generated Java model classes for processing the NS Infoplus data for train travel information in the Netherlands. 
Goal is to create a standard set of models that can be reused in JVM applications without resorting to generating your own from the WSDL/XSD.

This initial release contains models for just RIT as we test this library.

Supported
----
- **RIT** – These messages contain information about all the stops of a single train journey/service and any changes to it.

Usage
---
Add the following to your Maven configuration

```maven
<dependency>
  <groupId>nl.openov</groupId>
  <artifactId>infoplus-model-java</artifactId>
  <version>1.0-SNAPSHOT</version>
</dependency>
```

or Gradle
```gradle
  repositories {
      mavenCentral()
      maven {
          url = uri("https://maven.pkg.github.com/joelhaasnoot/infoplus-model-java")
      }
  }

  dependencies {
      implementation("nl.openov:infoplus-model:1.0-SNAPSHOT")
  }
```

TODO
---
- Publish to Github Packages
- DVS messages
- DAS messages
- Verstoringsinformatie: LAB, TRB, STB, VTT, VTL, VTS etc


Also see
---
- Alternative for Javascript: https://www.npmjs.com/package/travel-info-types
- NETEX: https://github.com/entur/netex-java-model
- SIRI: https://github.com/entur/siri-java-model
