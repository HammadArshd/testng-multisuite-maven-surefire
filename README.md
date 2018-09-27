# selenium-testng-Maven
Proof of Concept  Testng Suites Parallel Execution

mvn clean verify
- will pick <suiteXmlFile>src/test/resources/mkyong-testng.xml</suiteXmlFile> from properties


mvn clean verify -PmultiFile
-  will pick <suiteXmlFile>src/test/resources/mkyong-testng.xml,src/test/resources/conRefNvAL-testng.xml</suiteXmlFile> from profile "multiFile"

Command Line Execution
- mvn clean verify -Dsurefire.suiteXmlFiles=src/test/resources/conRefNvAL-testng.xml
- mvn clean verify -Dsurefire.suiteXmlFiles=src/test/resources/mkyong-testng.xml,src/test/resources/conRefNvAL-testng.xml

