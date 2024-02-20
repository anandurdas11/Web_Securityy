# Lab: File path traversal, traversal sequences stripped non-recursively #

## Lab Description ## 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ebaf9561-6270-4529-953f-fb50e7bf70f2)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/674d27fc-74d3-46e3-8d13-6f44742f4594)

> What is exactly means is that in previous labs we used the payload `../../../etc/passwd` when  the browser fliters       this it will not work we have to bypass for that we use differnet payload.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3350b529-4795-4b26-843f-f9920f9bb636)

> As in the pervious labs we wil open the image in new tab and replace the file name feild.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2e1b6001-d45a-4fe7-a829-6eb4d74b219b)

> Let's try usual payload.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a4f1e5da-0a2e-41a2-a842-1fa3b4b974a2)

> The attack was no success ful means the server flitering the input so we change the payload `....//....//....//etc/passwd` and try.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/dd2c6842-9f41-41c7-b8e0-8afb416e7c2d)

> We have changed the payload.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/61e0ab07-e344-4c5f-ac90-e0d7be0073c2)

> Now we are able to see the content of the `/etc/passwd` file.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/b88eff12-cef2-4059-ac66-1495d8e91a8c)


