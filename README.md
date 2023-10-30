# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.


![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/b9381141-d9e0-44c3-82de-4a48d700d92d)




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/4f0e342c-0251-469b-9f3e-e7a29c73304c)

 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/697307df-4e6e-4f64-ab7c-90d43929da77)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/0cd07f3f-1e48-4500-a63e-c99be0c4c3a4)

 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/f4b88eab-462a-4ab4-b10a-d2017e38ef48)





Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/9c5ffa48-6549-4627-b8b5-8cfdb3755f94)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/b94c924c-0772-4ac7-8333-1efa2308789a)



Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/3b767184-1d60-47fa-a940-c908f417eee9)

 
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/68ba2c1b-47a7-4c46-a98f-31e49f9e75d1)



Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/b97ddfb7-1e7c-437a-8fa7-ec25930659f6)

 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/674ad080-8bbd-41b2-b0f7-8d014c22889a)





Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
![image](https://github.com/chgeethika/Ex-04_RESTful_Web_Services/assets/142209368/ee20dca1-9130-43b8-8727-01a79a77e1cc)
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
