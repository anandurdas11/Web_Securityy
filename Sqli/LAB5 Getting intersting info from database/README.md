## Lab: SQL injection UNION attack, retrieving data from other tables ##

### Lab Description ###

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/89aac6b0-92a0-4c9e-a1b4-e366084ec919)

> So in this lab we have retrieve the username and password and login as administrator account.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/432c7c0b-e916-4da0-bc39-5d8cda0818e4)

So this target website.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7836222b-7f81-4662-a2d3-cd54252db91e)

> So try sql injection in this url and try to retrieve username and password

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fc2a416d-f272-499a-969d-05840927aa10)

> By injecting `' UNION SELECT username, password FROM users--` we were able to retreive the username and passowords.

> Now we will try to login with admin's details.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7c8b2558-930c-4021-9d0b-dbbdf53b77de)

> So we were able to sucessfully able to login as administrator.



