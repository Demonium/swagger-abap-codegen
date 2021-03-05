
# swagger-abap-codegen
abap generator for swagger

**Setup:**

Put file **AbapClientCodegen.java** in path below **swagger-codegen\modules\swagger-codegen\src\main\java\io\swagger\codegen\languages\
Add folder abap in path swagger-codegen\modules\swagger-codegen\src\main\resources\**

Add entry **io.swagger.codegen.languages.AbapClientCodegen** in the file located at **path swagger-codegen\modules\swagger-codegen\src\main\resources\META-INF\services\io.swagger.codegen.CodegenConfig**

**Version:**

java version : 1.8.0_271
mvn version : Apache Maven 3.6.3
Based on modules/swagger-codegen-cli/target/swagger-codegen-cli.jar version > 2.4.0-SNAPSHOT

**Build:**

Compile swagger with the command below : mvn clean package
execute with the command below


**Execute:**

java -jar modules/swagger-codegen-cli/target/swagger-codegen-cli.jar generate -i <API_FILE_OR_URL> --model-name-prefix ty_ -l abap  -o <OUTPUT_DIRECTORY>


**Debug:**

 - Debug operations

java -DdebugOperations -jar modules/swagger-codegen-cli/target/swagger-codegen-cli.jar generate -i <API_FILE_OR_URL> --model-name-prefix ty_ -l abap  -o <OUTPUT_DIRECTORY> > <PATH_TO_DEBUG_OPERATIONS_FILE>

 - Debug models

java -DdebugModels -jar modules/swagger-codegen-cli/target/swagger-codegen-cli.jar generate -i <API_FILE_OR_URL> --model-name-prefix ty_ -l abap -o <OUTPUT_DIRECTORY> > <PATH_TO_DEBUG_MODELS_FILE>
