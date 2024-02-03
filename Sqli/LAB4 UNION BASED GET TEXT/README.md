## Lab: SQL injection UNION attack, finding a column containing text ##

### Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ebd4fc04-da79-4283-87d7-13a45474eef0)

> So here we have to perform the union based sql injection attack method to retrieve the text data from the database.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e03c9599-28be-4266-8fc8-2a93d009caf8)

> So above is the target site we have to retrieve the string `Q7Oo45` from the database.

> When now the site is vulnerable to sql injection attack lets try `UNION` based payload to make the attack sucessful.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e335851f-0b7e-40d9-a5d5-1084082cd333)

> In the first attempt we try check for text data in `1` column but there no readable data in the first column so it gives internal server.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4658e0c2-2dce-4593-9fe9-401034e1cb7e)

> So what we did here was the repalce the string with string we have to retrieve and the string was present in `3` column.
  paylod ` ' UNION SELECT NULL,NULL,'Q7Oo45' -- `


 

