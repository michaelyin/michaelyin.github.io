---
layout: post
title: Upgrade Spring Boot to Version 1.2 in the rest service
---

Spring Boot 1.2 is just available. I update the REST service project with the new version. 

1. With upgrade of servlet-api version from 2.5 to 3.1.0 additional methods are required by classes extending javax.servlet.ServletInputStream. Need to override those methods.
2. In Eclipse, due to the upgrade of Spring Boot, you need to rebuild your classpath. Or run it in command line:
   gradle eclipse

