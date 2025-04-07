# Ex-02_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.


Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.

 ![278527664-8b9ef62c-82a7-4733-b94c-25f3dc5a9081](https://github.com/user-attachments/assets/7e957750-1235-4299-ae96-83b365fd734b)

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![278527696-aab0aa19-096e-44f2-997b-2bb9a46bec1d](https://github.com/user-attachments/assets/be654b94-88c1-4bf5-af46-d5fce3a432f3)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

![278527818-d8c3c728-3d2b-4991-91ee-664fe2a7257c](https://github.com/user-attachments/assets/2dd43d1e-f556-4dd7-b577-3162d395f472)

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).

![278527913-cf60de3c-6fc9-4310-9186-2f7e9d79585c](https://github.com/user-attachments/assets/210091f9-1502-4b24-90f3-b9443cd9863c)



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![278527936-69392b1c-9c4d-445a-880b-fe97a780640c](https://github.com/user-attachments/assets/4a9749cd-1280-4163-8570-25919504c09b)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.



Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 
![278528201-100a668b-4f71-47c2-bb5e-a454671e4efd](https://github.com/user-attachments/assets/9520de48-f431-45bf-9498-5f69892c7422)


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


![278528245-66462b76-62a4-42a3-9db0-237a605aec6a](https://github.com/user-attachments/assets/6a87d95f-0cd5-4cd0-8a77-8d4a2de002b4)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 

 ![278528272-a74cb20f-a6e4-43d0-b1e8-7176be82ae16](https://github.com/user-attachments/assets/f6a60e73-240c-4826-a398-6862a432a00d)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![278528310-e28d0aee-751b-4c96-a007-575b768e48e5](https://github.com/user-attachments/assets/cf8d290f-8ba9-48be-aef0-6c9b27021b48)

Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
![278528370-9876177d-c4ef-46f9-a459-1087d92d30b6](https://github.com/user-attachments/assets/98170ec6-0c5e-436d-b5cf-92ae13b8a38d)


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
