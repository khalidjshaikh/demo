Windows 11 x86-64
Java 24.0.1 
Spring Boot v4.0.0-SNAPSHOT
Tomcat 11.0.9

winget install --id Amazon.Corretto.24.JDK

java -version
openjdk version "24.0.1" 2025-04-15

choco install gradle # Run PowerShell as administrator.  Launch new shell.

gradle --version
Gradle 8.14.2

gradle bootRun

![](images\Screenshot 2025-07-08 145907.png)

---

Ubuntu 24.04 x86-64

java -version
openjdk version "21.0.7" 2025-04-15

# sudo apt install gradle
# gradle --version
# Gradle 4.4.1

curl -s "https://get.sdkman.io" | bash
source "/home/khalid/.sdkman/bin/sdkman-init.sh"
sdk i gradle # gradle 9.0.0-rc-1

sudo apt install gradle
gradle --version
Gradle 9.0.0-rc-1

gradle bootRun

----

Amazon Linux 2023.7.20250623

java -version
openjdk version "24.0.1" 2025-04-15

curl -s "https://get.sdkman.io" | bash
source "/home/khalid/.sdkman/bin/sdkman-init.sh"
sdk i gradle # gradle 9.0.0-rc-1

gradle --version
Gradle 9.0.0-rc-1

gradle bootRun

![](images\Screenshot 2025-07-08 232434.png)

---

The Spring Framework is a popular, open-source, lightweight framework for building Java enterprise applications

Spring Boot is an open-source, a microservice-based Java web framework offered by Spring, particularly useful for software engineers developing web apps and microservices. 

spring-boot-starter-web includes an embedded Tomcat server, allowing you to run your web application as a self-contained executable.

---

gradle bootRun

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::       (v4.0.0-SNAPSHOT)
2025-07-08T15:19:38.150-05:00  INFO 2984 --- [demo] [           main] com.example.demo.DemoApplication         : Starting DemoApplication using Java 24.0.1 with PID 2984 (C:\Users\khale\git\gradle-groovy\demo\build\classes\java\main started by khale in C:\Users\khale\git\gradle-groovy\demo)
2025-07-08T15:19:38.154-05:00  INFO 2984 --- [demo] [           main] com.example.demo.DemoApplication         : No active profile set, falling back to 1 default profile: "default"
2025-07-08T15:19:38.938-05:00  INFO 2984 --- [demo] [           main] o.s.boot.tomcat.TomcatWebServer          : Tomcat initialized with port 8080 (http)
2025-07-08T15:19:38.954-05:00  INFO 2984 --- [demo] [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2025-07-08T15:19:38.955-05:00  INFO 2984 --- [demo] [           main] o.apache.catalina.core.StandardEngine    : Starting Servlet engine: [Apache Tomcat/11.0.9]
2025-07-08T15:19:39.007-05:00  INFO 2984 --- [demo] [           main] b.w.c.s.WebApplicationContextInitializer : Root WebApplicationContext: initialization completed in 796 ms
2025-07-08T15:19:39.481-05:00  INFO 2984 --- [demo] [           main] o.s.boot.tomcat.TomcatWebServer          : Tomcat started on port 8080 (http) with context path '/'
2025-07-08T15:19:39.485-05:00  INFO 2984 --- [demo] [           main] com.example.demo.DemoApplication         : Started DemoApplication in 1.745 seconds (process running for 2.106)
<==========---> 80% EXECUTING [11s]
> :bootRun