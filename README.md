# Phase_3

1: Open Github link: https://github.com/

2: Clone directory on your local using code: git clone https://github.com/Utkarsh20th/Phase_3.git
   Note: Java code is build on Maven- all the dependencies are included in the project's POM.xml

3: Extract the project present in the clone directory

4: First folder will be of JMeter project
   - JMeter script will be present in folder: Phase_3/Code_JMeter/1_Script/Simplilearn.jmx
   - Open JMeter application and select "Open", give path where above file is located
   Load:
   * "Enable" JMeter element [jp@gc - Ultimate Thread Group (Load Testing)] to Load Testing
   * Press "Start" button for execution
   * Path to store the csv result of the execution can be given in the "Filename" section [OR] The csv results are located in folder: Phase_3/Code_JMeter/2_Result/Load/
   * Screenshots of the results are located in folder: Phase_3/Code_JMeter/3_Screenshots/Load/
   Spike:
   * "Enable" JMeter element [jp@gc - Ultimate Thread Group (Spike Testing)] to Spike Testing
   * Press "Start" button for execution
   * Path to store the csv result of the execution can be given in the "Filename" section [OR] The csv results are located in folder: Phase_3/Code_JMeter/2_Result/Spike/
   * Screenshots of the results are located in folder: Phase_3/Code_JMeter/3_Screenshots/Spike/
   Stress:
   * "Enable" JMeter element [jp@gc - Ultimate Thread Group (Stress Testing)] to Stress Testing
   * Press "Start" button for execution
   * Path to store the csv result of the execution can be given in the "Filename" section [OR] The csv results are located in folder: Phase_3/Code_JMeter/2_Result/Stress/
   * Screenshots of the results are located in folder: Phase_3/Code_JMeter/3_Screenshots/Stress/

5: Second folder will be of POSTMAN project
   - Open POSTMAN application
   - Click on "Import" --> select "Folder" option --> select "Choose folder from your computer" --> give path Phase_3/Code_POSTMAN/1_Script/Collection/Simplilearn_Phase_3_Assessment.postman_collection.json [OR] Click on "Import" --> select "Link" option --> the link is given present in file located at Phase_3/Code_POSTMAN/1_Script/Collection/
   - The Collection will be imported in the POSTMAN application. Expand the Collection to see GET and POST requests
     Note: GET operation is done to fetch list of users from Reqres.in API
           POST operation is done to add a user into Reqres.in API
   - Also import the necessary Environment variables. They are located at location Phase_3/Code_POSTMAN/1_Script/Environment/Simplilearn_Phase_3_Assessment_Environment.postman_environment.json
   GET
   * Click on "GET_(List_of_users)" and then click on "Send". The API response and the result of reponse validation will be seen in  "Response-Body" tab and "Test Results" tab respectively
   * Result is also stored at location Phase_3/Code_POSTMAN/2_Result/GET_Response.json
   * Screenshots of the execution and results are present at location Phase_3/Code_POSTMAN/3_Screenshots/GET/
   POST
   * Click on "POST_(Add_a_user)" and then click on "Send". The API response and the result of reponse validation will be seen in  "Response-Body" tab and "Test Results" tab respectively
   * Result is also stored at location Phase_3/Code_POSTMAN/2_Result/POST_Response.json
   * Screenshots of the execution and results are present at location Phase_3/Code_POSTMAN/3_Screenshots/POST/

6: Third folder will be of RESTAssured project

   - [Option 1]: Download Zipped Project (it will download the complete RESTAssured project workspace - no extra dependencies will be required to use)
   -           - goto path Phase_3/Code_ZIP_File_RESTAssured/Simplilearn_Phase_3_Assessment.zip
   -           - click on "View raw" or "Download"
   - DOWNLOAD the Maven project present at location Phase_3/Code_ZIP_File_RESTAssured/Simplilearn_Phase_3_Assessment.zip and into the Eclipse workspace
   - In "Package Explorer" tab of Eclipse, project name "Simplilearn_Phase_3_Assessment" will be seen as a directory folder, right-click the folder
   - and select Maven-->Update Project...
                GET
                   * double-click the java code (.java) file present in the directory at location
                     Simplilearn_Phase_3_Assessment\src\test\java\Project\Simplilearn_Phase_3_Assessment\GET_list_of_users.java
                   * select Run As --> 1 TestNG Test
                   * the (output + log) messages will be seen in console
                POST
                   * double-click the java code (.java) file present in the directory at location
                     Simplilearn_Phase_3_Assessment\src\test\java\Project\Simplilearn_Phase_3_Assessment\POST_adding_a_user.java
                   * select Run As --> 1 TestNG Test
                   * the (output + log) messages will be seen in console
   - after the execution, right-click the project folder "Simplilearn_Phase_3_Assessment" and click "Referesh", the latest execution reports will be generated
     at the location Simplilearn_Phase_3_Assessment\test-output
     [OR]
     the execution reports have been saved at location Phase_3/Code_RESTAssured/2_Response/Reports
     
   - [Option 2]: Download very few RESTAssured project related files
   -           - goto path Phase_3/Code_RESTAssured/1_Maven_Script/Simplilearn_Phase_3_Assessment/src/test/java/Project/Simplilearn_Phase_3_Assessment/
   -           - click on "GET_list_of_users.java" to get code on GET operation
   -           - click on "POST_adding_a_user.java" to get code on POST operation
