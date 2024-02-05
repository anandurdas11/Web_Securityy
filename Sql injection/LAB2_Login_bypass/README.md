## Lab: SQL injection vulnerability allowing login bypass ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9b4e2452-8995-48a9-a2a4-4326ca240bf4)

> So in this we are going to bypass the login screen get `administrator` account acess.
  We know the user name of the admin i.e `administrator` so with this detail we are going to
  bypass the login screen.

This the Login screen so here we have to enter the `username` and `password`.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/75d8600e-0d9a-46c6-915e-4ddf7b8af108)

> We know the sql query for a login form it goes like `SELECT username,password FROM users WHERE 
  username AND password`.

> So we will create a payload in such a way that only the username will be checked and password check will igonred.

> Like this we give username feild input `administrator'--` So what it will do is only username will be checked and 
  password checking will be commented and not checked and we will get the respective user account.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d0470315-fe9f-4472-9814-071fc7955697)

So using the payload we were sucessfully able login into the admin account!!!.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bb80ba6e-a107-4b8f-a88f-7e5dd6dfff71)

