## This exercise can be taken up after completion of Day-1 and Day-2 curriculum.

### Problem Statement

A bank has two organization (business units), namely 'Retail' and 'Wholesale'. They are looking to implement a multi-tenant deployment of API Connect to cater the needs of both the organizations. An API Connect instance has been deployed on a CP4I cluster and you have been tasked to appropriately configure the environments. Following requirements must be met:
      
       - API Manager needs to authenticate users from LDAP registry.
       - Both the organizations need isolated API management environments.
       - Owner of 'Retail' organization should be user 'vest1' from the LDAP registry.
       - Owner of 'Wholesale' organization should be user 'vest2' from the LDAP registry.
       - Users of the LDAP registry should be scoped to their API manager environment only 
         and should not have ability to manage/modify the API Connect cluster.
       - Add another user 'vest3' from Open LDAP as developer into both 'Retail' and 'Wholesale' organizations.
       - Both the organizations need to have their DEV and UAT environments.
       - Each environment needs to have their own developer portal.
       - Enable API lifecycle approval for 'Stage' and 'Published' states in both DEV and UAT environments. 
         for both the organizations. Enable 'Take self-approval' option for simplicity of this exercise.
       - In organization 'vest1', enable approval for self service onboarding for both DEV and UAT developer portals.
       - Logout and Login as user 'vest3' into API manager and select 'Retail' organization
       - Use the deposit API yaml definition (in the same way as you did hotelreview in lab1) to create an API in vest1. Secure it with the client-id and client-secret.
       - Use this as backend url for deposit API
         `http://deposit-http-ace.apps.ocp-060001q8qm-ada2.cloud.techzone.ibm.com/deposit/v1`
       - Create a product namely 'Deposit' and create two plans with the names 'Silver' and 'Gold'. Follow lab6 for directions.
       - Test this product in Sandbox environment
       - Publish this product to DEV env.
       - Publish this product to UAT env.
       - Onboard a consumer organiztion, namely 'Fintech' onto DEV environment's developer portal
       - Subscribe to the product and test from developer portal.
       - Test the API from Postman
       




### Hints
Use below information for configuring Open LDAP registry:

Create a new Open LDAP user registry in cloud manager. Open LDAP credentials will be provided by lab instructor. 

##### LDAP Server and port: Will be shared by the instructor
      
#### Authentication method: Compose DN
      
#### Admin DN: `cn=admin,dc=gsilab,dc=ibm,dc=com`
      
#### Password: Will be shared by the instructor
      
#### Prefix: `uid=`
      
#### Suffix: `,ou=People,dc=gsilab,dc=ibm,dc=com`
      

![](images/open_ldap_config.png)

