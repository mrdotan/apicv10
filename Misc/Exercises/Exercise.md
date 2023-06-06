## This exercise can be taken up after completion of Day-1 and Day-2 curriculum.

### Problem Statement

A bank has two business units, namely 'Retail' and 'Wholesale'. They are looking to implement a multi-tenant deployment of API Connect to cater the needs of both the business units. An API Connect instance has been deployed on a CP4I cluster and you have been tasked to appropriately configure the environments. Following requirements must be met:
      
       - API Manager needs to authenticate users from LDAP registry
       - Both the business units need isolated API management environments
       - Owner of 'Retail' business unit should be user 'vest1' from the LDAP registry
       - Owner of 'Wholesale' business unit should be user 'vest2' from the LDAP registry
       - Users of the LDAP registry should be scoped to their API manager environment only and should not have ability to manage/modify the API Connect cluster
       - Each of the business units need to have their DEV, UAT and PROD environments
       - Each environment needs to have their own developer portal
       - Enable API lif


* * Credentials for an Open LDAP server will be provided by the instructor. 

### Hints
Create this setup in your environment by following the below steps:

1) Create a new Open LDAP user registry in cloud manager. Open LDAP credentials will be provided by lab instructor. 

![](images/open_ldap_config.png)

2) 