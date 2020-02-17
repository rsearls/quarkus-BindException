# quarkus-BindException


Before running the test install this archive in your local repo.
Here is the cmd to do it.

mvn install:install-file \
   -Dfile=___FIX_THIS___/lib/utils-arquillian-utils-4.5.0-SNAPSHOT.jar \
   -DgroupId=org.jboss.resteasy \
   -DartifactId=utils-arquillian-utils \
   -Dversion=4.5.0-SNAPSHOT \
   -Dpackaging=jar 


  Compile project:
    mvn clean test -DskipTests=true
  
  Set breakpoint in ObserverImpl line 54 or in
  java.net.BindException line 47
  
  Run tests
    mvn test -Dmaven.surefire.debug