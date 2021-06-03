# ThycoticMuleIntegration
**Overview**
Thycotic Secret Server is a privileged account management solution designed specifically for IT admins and IT security professionals, helping them take charge and be in control of all password management-related processes across the enterprise. 

There are two ways to connect to Thycotic Secret Server via Mulesoft:-

**1. REST API**

**REST API Documentation**:- https://${YouSecretServerInstance}/Documents/restapi/

First step is to create trial account and trial instance on Thycotic Secret Server. Then move to Mulesoft coding.
The example in Mule project first calls the "/oauth2/token" API to get the access token. Then uses the access token to call "/users/current" to get the list of current users from Thycotic Secret Server.


**2. SOAP**

**SOAP Documentation** :- https://${YourSecretServerInstance}/webservices/SSWebservice.asmx

The example in Mule project first calls the "Authenticate" webservice to get the access token. Then uses the access token to call "GetTokenIsValid" to validate the access token.
