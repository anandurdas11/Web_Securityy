# Lab: Basic SSRF against another back-end system #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3dbe66d0-ba47-42b9-8522-448a08b11149)

## Target machine ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e15cddaa-f75c-4d9e-9b03-b63ce506dd32)

> We intercept the request and change the stockapi part

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3228b25c-019b-4a25-abf4-b72dcea36466)

> When changed the stockapi value but it's giving some error

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/23290ce0-3317-4e21-9f84-c976fa788fde)

> Now we will try to guess the exact parameter

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a618cf16-709f-4e46-9cfc-7bd43c167771)

> Now we start the brute force attack

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/98b1c185-0865-42ce-8a5a-24d649d99408)

> We have set the payload

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/81b110e7-ab96-4a66-895a-6db3e4602fa5)

> so we can see that the corrected payload `http://192.168.0.52:8080/admin` now change payload to delete user carlos

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/35a940b9-4824-465b-9631-342568a5bf70)

> For deleting the user carlos we change payload to `http://192.168.0.52:8080/admin/delete?username=carlos`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/38715e7c-219b-45fa-84e2-d91b1b4c2567)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/82b8b323-0d33-49aa-aab9-4d056e942a02)


