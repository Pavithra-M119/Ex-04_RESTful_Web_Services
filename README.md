# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/739b75a0-758f-44b9-9ca5-f961f15e773c)




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/43810d23-3749-43d1-82a9-ee1a939dbbbd)
 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/4ce1bafa-be29-44fc-b85e-a50739b0ec6d)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.

 ![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/aa6f0fe0-c4e1-445f-8441-b28c74fa725b)


 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/b81d4649-d7d4-48d8-a49c-d0c724977b50)




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/204c9b80-7d4b-448f-ace4-b8236c6a9fe3)



 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/bcf63622-f32a-4d2f-812e-7f099381df9f)


Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/a8248177-1e55-4c89-8dd1-6cfb8833c7ff)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/fa0b86c0-86a3-4206-9dc0-650c7bccb1ce)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/ae39fea3-1614-4e93-abf4-831b257d704b)
 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/8e43f9af-8564-4834-bab6-d0ab026650c7)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.

![image](https://github.com/Pavithra-M119/Ex-04_RESTful_Web_Services/assets/119229774/8c18ee2c-99d7-4732-9214-bf850cc576c9)
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
