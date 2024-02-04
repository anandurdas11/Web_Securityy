## Lab: SQL injection attack, querying the database type and version on MySQL and Microsoft ##

### Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/094a7bf4-2219-4d1a-a9b2-f6ee64b78d5d)

> So we have to get the database information.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1d9bbf4b-73c1-4dc0-8fb7-30039f835db6)

> So the above is the target website we have get the database info from the database.

> So we tried the sql injection with payload `' UNION SELECT @@version--` it give internal server error.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/323f91f4-6304-44df-af33-8ea9ae44bd13)

> So when we tried with `' UNION SELECT @@version,NULL--1` it worked there is second column too.
