# CAS Drupal 7 Module for UNI Authentication

This is a package of the CAS Drupal 7 Module plus phpCAS for Columbia University Network Identifier (UNI) Authentication on Drupal sites. 

You MUST register your URL as a service with CUIT Identity and Access Management before you can successfully authenticate via CAS. Please follow the instructions from CUIT IDM to register your service before installing and configuring this module: http://cuit.columbia.edu/cas-authentication

## Configuration

1. Install the CAS Module.

2. Navigate to /admin/config/people/cas to configure the Module.

3. In "Library (PHPCAS)" section, enter CAS-1.3.2 in the Library directory field.

4. In "CAS Server" section, select the "SAML Version 1.1" radio button.

5. Under the "Hostname" field, enter the dev or production hostname URL as specified by CUIT IDM (e.g. casdev.cc.columbia.edu).

6. Under the "Port" field, enter 443.

7. Under the "URI" field, enter /cas.

8. Configure the "Login Form" section as desired.

9. Configure the "User Accounts" section as desired. Please note that the "Automatically create Drupal accounts" checkbox is selected by default. In production environments, this should probably be unchecked for security reasons.

10. Under the "Redirection" section, check the "Check with the CAS server..." box if you have your service configured for SSO.

11. Configure the "Require CAS Login for" section for the pages you wish to secure with UNI authentication.

12. All of the other settings are optional.