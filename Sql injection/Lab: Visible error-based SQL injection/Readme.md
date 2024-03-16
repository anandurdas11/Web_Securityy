# Lab: Visible error-based SQL injection #

# Lab Description #

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e664960c-6556-4b17-9ff6-0c26a8b8f454)

> We have to get the password and login as admin

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/53d17410-9cb9-450a-811d-601193fdf8d6)

> Above is the target website

> We have intercepted the request going to login page and now we will try manipulate request

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3eee12d1-40a8-4fef-a44f-44c37d02f115)

> so we put `'` after the trackin id it's giving error so sql injection is possible.
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/07d27f84-6423-4df7-9e65-2bc321a5adf1)

> When we commented the query using `'--` we query was sucessful
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e7c1a7cc-2f4e-49c0-9ddd-7e80668d2d16)
> `' AND 1=CAST((SELECT username FROM users) AS int)--` it gives some literal because we have reached some kind of
   length limit lets remove the tracking Id and try

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ce3563fe-3503-4796-933a-6408c8bcc589)

> This query is giving a some error that more than 1 row is selecte we have row limit to 1

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bc5d2d3b-f58d-457d-a143-ebe59898059b)

> We are getting the username as administrator. So we can confirm that first row contain details of admin

> Now we try to extract password using payload `' AND 1=CAST((SELECT password FROM users LIMIT 1) AS int)--`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/54ca2b52-58ae-4b61-ad9b-18ebceb98de9)

> We got the password `yzdzerrej92rrbk13t3a` lets try to login with this.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fa879d61-0b76-42ef-8746-56a4d25955bc)
