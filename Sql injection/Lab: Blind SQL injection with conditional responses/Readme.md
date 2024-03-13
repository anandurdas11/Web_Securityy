![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fb5a8ae4-ccb3-498e-ad97-24ece925a11b)# Lab: Blind SQL injection with conditional responses #

# Lab Description #

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/74e7b715-abf7-407e-9f47-d2ac92fef4f3)

> We have intercepted the request using the burpsuite

  ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c5633966-195e-48f2-a86c-9c30715442a3)

> We send this to repeater

> We firts use the payload `' AND '1'='1` and checking whether the welcome back message comming or not

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a98bc57f-6772-4ebc-99e2-074d7c355395)

> And we can see that welcome back message is coming

Again we will change the payload `' AND '1'='2` checking whether the error is reflected or not

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7e536a9b-34d7-4417-80f1-03d145239116)


> In this we can see that welcome back is not showing

> Let's use this payload to select the user with name starting  with a `' AND (SELECT 'a' FROM users LIMIT 1)='a`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/14eeba98-e49a-4f72-bee9-bba9eade506b)

> So we can see that welcome back is reflected so there username with letter a let's check whether it admin or not

> `' AND (SELECT 'a' FROM users WHERE username='administrator')='a` will return a if adminstrator is there so it's true

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/140454c8-5f1d-4ef3-9183-000d0d6bcc77)

> Let's check the password length `' AND (SELECT 'a' FROM users WHERE username='administrator' AND LENGTH(password)>1)='a` with this payload

 By brute we came to know password length is 20

> By brute force we found that first letter is 6

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/57c63097-f321-4faf-b7b2-c91744c133ef)

> For finding the final password we will bruteforce

> We got the password

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e01146f5-ab23-4a0f-b89b-20a50df43140)

> password `6n6qynt8ypnmxan814k9`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ab9ea0f4-9acc-4795-bc32-000c14058f71)

