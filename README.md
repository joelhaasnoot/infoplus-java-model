infoplus-java-model
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
  <artifactId>infoplus-java-model</artifactId>
  <version>1.0-SNAPSHOT</version>
</dependency>
```

or Gradle
```gradle
  repositories {
      mavenCentral()
      maven {
          url = uri("https://maven.pkg.github.com/joelhaasnoot/infoplus-java-model")
      }
  }

  dependencies {
      implementation("nl.openov:infoplus-java-model:1.0-SNAPSHOT")
  }
```

TODO
---
- DVS messages
- DAS messages
- Verstoringsinformatie: LAB, TRB, STB, VTT, VTL, VTS etc


Also see
---
- Alternative for Javascript: https://github.com/InterlockedSim/travel-info-types

Other transit models in Java
---
- NETEX: https://github.com/entur/netex-java-model
- SIRI: https://github.com/entur/siri-java-model
- BISON KV6 https://github.com/bliksemlabs/kv6-java-model
- BISON KV15 https://github.com/bliksemlabs/kv15-java-model
- BISON KV17 https://github.com/bliksemlabs/kv17-java-model
- BUSON KV4 https://github.com/bliksemlabs/kv4-java-model
