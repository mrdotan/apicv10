## Use Case driven exercise - Banking Use Case

#### This exercise should be done after [ConfigureDeveloperToolkitExercise](https://github.com/ibm-ecosystem-lab/APICv10/blob/main/Misc/Exercises/ConfigureDeveloperToolkitExercise.md)

### Problem Statement

A bank is looking to implement API lifecycle management using IBM API Connect. You have been tasked to appropriately configure API Connect topology to support various environments, like DEV, UAT, PROD etc. You are supposed to configure two non-production environments, namely DEV and UAT on an API Connect instance.
Note the following requirements and steps:
      
       - The organization should support 'DEV' and UAT environments in addition to the Sandbox environment.
       
       - All the environments, namely Sandbox, DEV and UAT, should have their developer portals.
       
       - API Developers will develop APIs using API Connect developer toolkit locally and should have ability
         to publish and test in Sandbox environment.
       
       - API Developers should have ability to 'Stage' the products onto DEV and UAT environments.
       
       - Administrators can review & approve the products to publish to DEV and UAT environments.
         
       - A user with name 'developer' exists in the openldap registry. Assign this user 'Developer' role
         in the provider organization.
         
       - Start API Connect Developer Toolkit and connect to your provider organization using the provided credentials 
         for 'developer' user. Ensure that you have selected the correct provider organization (assigned to you)
         in the toolkit.
         
       - 
       
       - Each environment needs to have their own developer portal.
       
       - Enable API lifecycle approval for 'Stage' and 'Published' states in both DEV and UAT environments 
         for both the organizations. Enable 'Take self-approval' option for simplicity of this exercise.
         
       - In organization 'Retail', enable approval for self service onboarding for both DEV and UAT developer portals.
       
       - Logout and Login as user 'vest3' into API manager and select 'Retail' organization
       
       - Use the deposit API definition (look at the link to deposit.yaml below under 'Hints') to create an API 
         in 'Retail'. Secure it with the client-id and client-secret. (You can follow the steps from Lab1 for guidance)
       
       - Use the below as backend url for deposit API
         http://deposit-http-ace.apps.ocp-060001q8qm-ada2.cloud.techzone.ibm.com/
         
       - Create a product namely 'Deposit' and create two plans with the names 'Silver' and 'Gold'. Follow 
         lab6 for directions.
       
       - Test this API in Sandbox environment
       
       - Stage this product to DEV env while you are logged in as 'vest3' user. Try to publish it.
       
       - Logout and login as user 'vest1'. Now approve this product and publish.
       
       - Stage and Publish this product to UAT env.
       
       - Onboard a consumer organization, namely 'Fintech' onto DEV environment's developer portal
       
       - Create a consumer application, namely 'BestDeposits'
       
       - Subscribe to the product and test from developer portal.
       
       - Test the API from Postman
       




### Hints
1) Instructor will provide you the API Manager Platform api url to connect from developer toolkit.

2) Instructor will provide credentials for the 'developer' user in openldap

3) [deposit.yaml](https://github.com/ibm-ecosystem-lab/APICv10/blob/main/Misc/Exercises/deposit.yaml) can be downloaded from here.

