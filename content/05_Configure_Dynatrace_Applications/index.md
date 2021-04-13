## Configure Dynatrace Application

This lab exercise will create a Dynatrace application for the Sock Shop application that was deployed. 

### Create Application
1.  Navigate to Applications and then select "My Web Application".
 
 ![Applications](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-applications.png)
 
2.  This is the default application bucket that catches all URLs for servers and services that are instrumented with Dynatrace. Scroll towards the bottom to "Top x Include Domains".
 
  ![Applications1](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-applications1.png)
  
3. Click on View Details
   - Both dev and prod Sock Shop domains are listed. They should match what you copied to notepad.
  
   ![Applications2](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-applications1b.png)
   
4. Expand the domain and click on "Create New Application".

   ![TransferDomain](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-transferdomain.png)
   
5. Click "Create"
   
   ![CreateApplication](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-createapplication.png)
   
6. Navigate back to Application in the Dynatrace menu and select Applications. Select the application you just created. You will see the application is named by the domain selected. Once you have selected the application, use the elypsis and select edit.

   ![EditApplication](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-editapplication.png)
   
7. Rename the application to DEV-Sock Shope or PROD-Sock Shop depending what application environment you are setting up first. Remember the environment names were based on the domain names and that is why we are changing them. 
   - When finished with the new naming, select the menu item for "Async Web Requests and SPAs".

   ![EditApplication](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-editapplication1.png)

8. Dynatrace automatically detect the jquery framework. Toggle the switch for jquery to the on position. 
   - Click on "Save".

   ![EditApplication](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-editapplication2.png)
   
9. Visit the Sock Shop and run transactions

10. Navigate back to Applications on the Dynatrace menu and select the newly named application.
   - Repeat these same steps for creating the production application.
   
   ![EditApplication](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/lab5-applicationview.png)
