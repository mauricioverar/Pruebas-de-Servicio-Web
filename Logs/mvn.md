```powershell
mvn clean test
[INFO] Scanning for projects...
[INFO] 
[INFO] --------------------< cl.kibernumacademy:test-rest >--------------------
[INFO] Building test-rest 1.0-SNAPSHOT
[INFO]   from pom.xml
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- clean:3.2.0:clean (default-clean) @ test-rest ---
[INFO] Deleting C:\Users\mvera\Documents\apirest\rest_assured\test-rest\target
[INFO]
[INFO] --- resources:3.3.1:resources (default-resources) @ test-rest ---
[INFO] Copying 0 resource from src\main\resources to target\classes
[INFO]
[INFO] --- compiler:3.13.0:compile (default-compile) @ test-rest ---
[INFO] Recompiling the module because of changed source code.
[INFO] Compiling 1 source file with javac [debug target 17] to target\classes
[INFO] 
[INFO] --- resources:3.3.1:testResources (default-testResources) @ test-rest ---
[INFO] skip non existing resourceDirectory C:\Users\mvera\Documents\apirest\rest_assured\test-rest\src\test\resources
[INFO]
[INFO] --- compiler:3.13.0:testCompile (default-testCompile) @ test-rest ---
[INFO] Recompiling the module because of changed dependency.
[INFO] Compiling 6 source files with javac [debug target 17] to target\test-classes
[INFO] 
[INFO] --- surefire:3.2.5:test (default-test) @ test-rest ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running cl.kibernumacademy.test.ProductCrudTest
Request URI:    http://localhost:8080/api/v1/products
Request URI:    http://localhost:8080/api/v1/products/2
Request URI:    http://localhost:8080/api/v1/products/2
Request URI:    http://localhost:8080/api/v1/products
Request URI:    http://localhost:8080/api/v1/products/2
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.904 s -- in cl.kibernumacademy.test.ProductCrudTest
[INFO] 
[INFO] Results:
[INFO]
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  4.259 s
[INFO] Finished at: 2025-09-02T18:02:15-04:00
[INFO] ------------------------------------------------------------------------
```